# Testing and Validation

## Objective

Validate that the WordPress deployment functions correctly after provisioning.

---

## Test Cases

### Test 1 – Instance Status

**Action**

Verify the Lightsail instance is running.

**Expected Result**

Instance status displays **Running**.

**Result**

Passed

---

### Test 2 – Website Accessibility

**Action**

Open the Static IP in a web browser.

**Expected Result**

The WordPress homepage loads successfully.

**Result**

Passed

---

### Test 3 – WordPress Administration

**Action**

Log in to `/wp-admin`.

**Expected Result**

The WordPress Dashboard loads successfully.

**Result**

Passed

---

### Test 4 – Content Publishing

**Action**

Create and publish a test blog post.

**Expected Result**

The post is visible on the public website.

**Result**

Passed

---

### Test 5 – Static IP Validation

**Action**

Verify the assigned Static IP remains attached.

**Expected Result**

The website is consistently accessible using the assigned Static IP.

**Result**

Passed

---

## Validation Summary

The deployment was successfully validated and met the functional requirements for a production-ready WordPress blog.