![AWS](https://img.shields.io/badge/AWS-Lightsail-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-6.x-21759B?style=for-the-badge&logo=wordpress&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Apache](https://img.shields.io/badge/Web_Server-Apache-D22128?style=for-the-badge&logo=apache&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MariaDB](https://img.shields.io/badge/Database-MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)

# Production-Ready WordPress Hosting on AWS Lightsail

> A production-ready WordPress deployment on AWS Lightsail demonstrating secure application hosting, static IP networking, backup planning, operational validation, and production hardening best practices.

---

## Project Overview

This project demonstrates how to deploy and manage a WordPress application using **AWS Lightsail**, a simplified virtual private server (VPS) service designed for small to medium-sized workloads.

The deployment focuses on building a reliable and cost-effective hosting solution while applying cloud engineering best practices such as static IP assignment, disaster recovery planning, operational validation, and security hardening.

Unlike a serverless static website hosted on Amazon S3 and CloudFront, this solution supports dynamic content management, user authentication, media uploads, and database-driven applications.

---

## Business Problem

A technology startup requires a company blog where employees can publish articles, tutorials, product announcements, and company updates.

The solution must:

- Deploy quickly with minimal configuration
- Minimize infrastructure management
- Provide predictable monthly costs
- Support WordPress content management
- Maintain persistent storage
- Support backups and disaster recovery
- Be scalable for future business growth

---

## Solution Architecture

```
                    Internet Users
                           │
                           ▼
                 Domain Name (Future)
                           │
                           ▼
                    DNS Resolution
                           │
                           ▼
                 AWS Lightsail Static IP
                           │
                           ▼
              AWS Lightsail WordPress Instance
        ┌─────────────────────────────────────┐
        │ Ubuntu Linux                        │
        │ Apache Web Server                   │
        │ PHP                                │
        │ WordPress                          │
        │ MariaDB                            │
        └─────────────────────────────────────┘
                           │
                           ▼
                 Lightsail Snapshots
```

A professional Draw.io architecture diagram is included in the `architecture/` directory.

---

## Why AWS Lightsail?

AWS Lightsail was selected because it provides:

- Rapid deployment
- Fixed monthly pricing
- Pre-configured WordPress environment
- Simplified networking
- Built-in snapshot capability
- Static IP support
- Reduced operational complexity

For small business websites and blogs, Lightsail offers a faster and more cost-effective deployment than configuring an Amazon EC2 instance from scratch.

---

## AWS Services Used

| Service | Purpose |
|----------|---------|
| AWS Lightsail | Virtual server hosting |
| Lightsail WordPress Blueprint | Pre-configured WordPress environment |
| Lightsail Static IP | Persistent public IP address |
| Lightsail Snapshots | Backup and disaster recovery |

---

## Project Structure

```
aws-wordpress-lightsail/
│
├── README.md
├── LICENSE
│
├── architecture/
│   ├── architecture.drawio
│   └── architecture.png
│
├── docs/
│   ├── implementation.md
│   ├── testing.md
│   ├── troubleshooting.md
│   ├── security.md
│   ├── cost-analysis.md
│   └── lessons-learned.md
│
├── screenshots/
│
└── scripts/
```

---

## Features

- WordPress deployment on AWS Lightsail
- Static IP configuration
- Persistent hosting environment
- Snapshot recovery strategy
- WordPress administration
- Operational validation
- Production-oriented architecture
- Low operational overhead
- Predictable monthly pricing

---

## Deployment Summary

The deployment consisted of the following high-level steps:

1. Create a Lightsail WordPress instance.
2. Verify successful deployment.
3. Allocate and attach a Static IP.
4. Access the WordPress administration portal.
5. Perform initial WordPress configuration.
6. Review backup strategy using Lightsail Snapshots.
7. Validate website functionality.
8. Document operational procedures.

Detailed implementation instructions are available in:

```
docs/implementation.md
```

---

## Validation

The deployment was successfully validated through the following tests:

- Lightsail instance status
- Website accessibility
- WordPress administrator login
- Static IP assignment
- Blog publishing functionality
- Deployment verification

Complete testing documentation is available in:

```
docs/testing.md
```

---

## Security Considerations

Security improvements implemented include:

- AWS-managed WordPress deployment
- Static IP networking
- WordPress updates
- Removal of default content
- Snapshot recovery planning
- Operational hardening

Planned enhancements include:

- HTTPS using Let's Encrypt
- Custom domain
- CloudFront integration
- AWS WAF
- Monitoring and alerting

Additional security documentation is available in:

```
docs/security.md
```

---

## Cost Optimization

AWS Lightsail provides predictable monthly pricing, making it well suited for startups, personal projects, and small business websites.

Cost optimization strategies include:

- Selecting the smallest suitable instance
- Removing unused snapshots
- Scaling only when required
- Using fixed-cost infrastructure

Detailed cost analysis is available in:

```
docs/cost-analysis.md
```

---

## Disaster Recovery

The disaster recovery strategy is based on **Lightsail Snapshots**.

Snapshots provide point-in-time backups that allow the entire server to be restored following events such as:

- Failed software updates
- Plugin failures
- Server corruption
- Configuration errors

Restoring the complete instance ensures operating system, web server, database, application, and configuration files remain consistent.

---

## Current Limitations

The current deployment intentionally reflects a learning environment.

Current limitations include:

- No registered custom domain
- HTTPS pending domain registration
- Single-instance architecture
- No automatic scaling
- No load balancing
- No CDN integration

These enhancements are identified as future improvements.

---

## Future Improvements

Future production enhancements include:

- Register a custom domain
- Configure HTTPS using Let's Encrypt
- Enable automatic snapshots
- Configure CloudFront
- Deploy AWS WAF
- Implement monitoring and alerting
- Automate deployments using GitHub Actions
- Manage infrastructure using Terraform
- Migrate to Amazon EC2 and Amazon RDS as traffic grows

---

## Screenshots

The `screenshots/` directory contains deployment evidence, including:

- Lightsail instance overview
- Running instance
- Static IP configuration
- Networking configuration
- WordPress homepage
- WordPress Dashboard
- Test blog post
- Snapshot configuration

---

## Lessons Learned

This project reinforced several important cloud engineering concepts, including:

- Differences between AWS Lightsail and Amazon EC2
- Static IP networking
- WordPress deployment and management
- Backup and disaster recovery planning
- Operational validation
- Production hardening
- AWS Shared Responsibility Model

Complete reflections are available in:

```
docs/lessons-learned.md
```

---

## Skills Demonstrated

- AWS Lightsail
- WordPress Administration
- Linux Server Management
- Static IP Networking
- Backup and Disaster Recovery
- Operational Validation
- Production Hardening
- Cost Optimization
- Technical Documentation
- Git & GitHub

---

## Repository Documentation

Additional technical documentation is available in the `docs/` directory:

- Implementation Guide
- Testing & Validation
- Troubleshooting Guide
- Security Review
- Cost Analysis
- Lessons Learned

---

## Author

**simeon siaka**

Cloud Engineer | AWS | DevOps | Infrastructure Engineering

Building production-ready cloud solutions through hands-on projects while documenting architecture, implementation decisions, operational procedures, and AWS best practices.