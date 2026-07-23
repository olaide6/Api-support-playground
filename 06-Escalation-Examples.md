# Escalation Examples

## Introduction

Not every customer issue can be resolved by the Product Support team.

When an issue is caused by a system bug, server outage, or requires code changes, it should be escalated to the Engineering team.

A good escalation provides enough information for engineers to investigate the issue efficiently.

---

# When Should You Escalate?

Escalate an issue when:

- The problem cannot be resolved through normal troubleshooting.
- Multiple customers are experiencing the same issue.
- An API returns repeated 5xx server errors.
- A bug has been confirmed.
- The issue requires changes to the application or infrastructure.

---

# Escalation Example 1 – Login Failure

## Customer Issue

> "I can't log into my account."

### Investigation

- Customer account verified.
- Password reset attempted.
- Browser cache cleared.
- Login API tested.
- API returned **500 Internal Server Error**.

### Escalation Summary

**Issue:** Login API returning 500 Internal Server Error.

**Impact:** Customer unable to access account.

**API Response:** 500 Internal Server Error.

**Steps to Reproduce:**

1. Enter valid login credentials.
2. Click **Login**.
3. Request fails with 500 error.

**Priority:** High

---

# Escalation Example 2 – Payment Service Failure

## Customer Issue

> "My payment won't go through."

### Investigation

- Payment details verified.
- Customer attempted payment multiple times.
- Payment API returned **503 Service Unavailable**.

### Escalation Summary

**Issue:** Payment service unavailable.

**Impact:** Customers cannot complete payments.

**API Response:** 503 Service Unavailable.

**Priority:** Critical

---

# Escalation Example 3 – Application Performance

## Customer Issue

> "The application is extremely slow."

### Investigation

- Issue confirmed by multiple customers.
- Network connectivity verified.
- API response time significantly delayed.

### Escalation Summary

**Issue:** High API response latency.

**Impact:** Slow application performance for multiple users.

**Priority:** High

---

# Best Practices for Escalation

Always include:

- Customer ID or Email
- Date and time of the issue
- Steps to reproduce
- Error message
- HTTP status code
- Screenshots (if available)
- Business impact
- Troubleshooting steps already completed

This information helps Engineering investigate the issue faster.

---

# Key Takeaways

✔ Escalate only after completing basic troubleshooting.

✔ Include clear and accurate technical information.

✔ Document every troubleshooting step.

✔ Explain the customer impact.

✔ Good escalations reduce resolution time and improve collaboration between Support and Engineering.

---

## Conclusion

Effective escalation is an important Product Support skill. Providing complete and accurate information helps Engineering identify the root cause more quickly, leading to faster resolutions and a better customer experience.
