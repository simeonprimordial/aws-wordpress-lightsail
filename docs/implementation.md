# Implementation Guide

## Objective

Deploy a production-ready WordPress application on AWS Lightsail using the managed WordPress blueprint while following AWS best practices for networking, backups, security, and operational readiness.

---

## Prerequisites

- AWS Account
- AWS Lightsail enabled
- Internet connection
- Git and GitHub repository
- Basic understanding of WordPress

---

## AWS Services Used

- AWS Lightsail
- Lightsail Static IP
- Lightsail Snapshots
- WordPress Blueprint

---

## Deployment Steps

### Step 1 – Create the Lightsail Instance

- Navigate to AWS Lightsail.
- Select **Linux/Unix**.
- Choose the **WordPress** blueprint.
- Select an appropriate instance plan.
- Name the instance `wordpress-prod-01`.
- Launch the instance.

---

### Step 2 – Verify Deployment

- Wait for the instance to enter the **Running** state.
- Access the public IP in a browser.
- Confirm that the default WordPress page loads successfully.

---

### Step 3 – Configure Static IP

- Allocate a Static IP.
- Attach it to the Lightsail instance.
- Verify that the website remains accessible.

---

### Step 4 – Log in to WordPress

- Access `/wp-admin`.
- Retrieve the administrator credentials.
- Log in successfully.

---

### Step 5 – Initial Hardening

- Update WordPress.
- Remove sample content.
- Configure site title and timezone.
- Review installed plugins and themes.

---

### Step 6 – Review Backup Strategy

- Review Lightsail Snapshots.
- Understand manual and automatic snapshot capabilities.
- Document the disaster recovery approach.

---

## Outcome

A fully functional WordPress application was deployed with a Static IP, validated, and prepared for future production enhancements such as HTTPS, a custom domain, and automated backups.