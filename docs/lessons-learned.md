# Lessons Learned

## Technical Lessons

During this project, I gained practical experience with:

- Deploying WordPress using AWS Lightsail.
- Configuring a Static IP.
- Understanding the importance of persistent networking.
- Validating a production deployment.
- Reviewing disaster recovery strategies using snapshots.
- Comparing AWS Lightsail with Amazon EC2.

---

## Architectural Lessons

This project demonstrated that AWS service selection should be driven by business requirements.

For a small business blog requiring rapid deployment and predictable costs, AWS Lightsail is a more suitable solution than Amazon EC2 due to its simplicity and reduced operational overhead.

---

## Operational Lessons

- Validate deployments before handing them over to users.
- Plan backup and recovery strategies before failures occur.
- Keep software updated.
- Document deployment decisions and operational procedures.

---

## Future Improvements

- Configure HTTPS using Let's Encrypt.
- Register a custom domain.
- Enable automated snapshots.
- Add monitoring and alerting.
- Introduce CloudFront for improved global performance.
- Migrate to an EC2-based architecture if scaling requirements increase significantly.