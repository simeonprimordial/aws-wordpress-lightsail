# Troubleshooting Guide

## Issue 1

### Website does not load

**Possible Cause**

- Instance is stopped
- Static IP not attached
- Firewall configuration

**Resolution**

- Start the Lightsail instance.
- Verify the Static IP assignment.
- Confirm ports 80 and 443 are open.

---

## Issue 2

### Unable to log in to WordPress

**Possible Cause**

Incorrect administrator credentials.

**Resolution**

Retrieve the administrator credentials using the Lightsail WordPress deployment instructions and retry.

---

## Issue 3

### WordPress Dashboard is slow

**Possible Cause**

Limited instance resources.

**Resolution**

- Monitor resource usage.
- Enable caching.
- Upgrade the Lightsail plan if required.

---

## Issue 4

### Lost access after restarting the instance

**Possible Cause**

Static IP not configured.

**Resolution**

Allocate and attach a Static IP.

---

## Issue 5

### Plugin update breaks the website

**Possible Cause**

Plugin incompatibility.

**Resolution**

Restore the Lightsail instance from the latest snapshot.