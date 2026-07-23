# Real Support Cases

## Introduction

Product Support Engineers investigate customer issues, identify the root cause, and either resolve the issue or escalate it to Engineering.

The following examples simulate common customer support scenarios.

---

# Case 1 – Customer Cannot Log In

## Customer Report

> "I can't log into my account."

### Investigation

- Confirmed customer's email address.
- Asked customer for the exact error message.
- Asked when the issue started.
- Tested the Login API.
- API returned **401 Unauthorized**.

### Root Cause

The customer entered incorrect login credentials.

### Resolution

- Guided the customer through resetting their password.
- Customer successfully logged in.

### Outcome

Issue resolved without Engineering involvement.

---

# Case 2 – Password Reset Email Not Received

## Customer Report

> "I requested a password reset, but I never received the email."

### Investigation

- Verified customer's email address.
- Asked customer to check Spam and Junk folders.
- Tested Password Reset API.
- API returned **200 OK**.

### Root Cause

The customer entered an incorrect email address.

### Resolution

Updated the email address and resent the password reset email.

### Outcome

Issue resolved.

---

# Case 3 – Payment Failed

## Customer Report

> "My payment keeps failing."

### Investigation

- Confirmed payment details.
- Checked payment gateway.
- Tested Payment API.
- API returned **503 Service Unavailable**.

### Root Cause

Temporary payment service outage.

### Resolution

Explained the issue to the customer.

Escalated to Engineering.

### Outcome

Engineering restored the payment service.

Customer successfully completed payment.

---

# Case 4 – Customer Cannot Update Profile

## Customer Report

> "I can't save changes to my profile."

### Investigation

- Verified customer account.
- Tested Update Profile API.
- API returned **403 Forbidden**.

### Root Cause

Customer account lacked the required permissions.

### Resolution

Updated account permissions.

Customer successfully updated profile.

### Outcome

Issue resolved.

---

# Case 5 – Application Loading Slowly

## Customer Report

> "The app keeps loading forever."

### Investigation

- Confirmed multiple customers were affected.
- Tested API response.
- API returned **500 Internal Server Error**.

### Root Cause

Backend service failure.

### Resolution

Collected logs and screenshots.

Escalated to Engineering.

### Outcome

Engineering fixed the issue and restored the service.

---

# Key Takeaways

✔ Investigate before escalating.

✔ Gather enough information before contacting Engineering.

✔ API responses help identify the root cause.

✔ Clear communication improves customer experience.

✔ Documentation speeds up issue resolution.

---

**Next:** [06-Escalation-Examples.md](./06-Escalation-Examples.md)
