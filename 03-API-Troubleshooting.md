# API Troubleshooting

## Introduction

One of the primary responsibilities of a Product Support Engineer is investigating customer issues before escalating them to Engineering.

API troubleshooting helps determine whether a problem is caused by customer input, application configuration, network connectivity, or the server itself.

---

# Troubleshooting Workflow

When a customer reports an issue:

Customer reports an issue

↓

Understand the problem

↓

Ask clarifying questions

↓

Attempt to reproduce the issue

↓

Check API response

↓

Identify HTTP Status Code

↓

Resolve or Escalate

---

# Example 1 – Customer Cannot Log In

### Customer Report

> "I can't log into my account."

### Investigation Checklist

- Verify the customer's email address.
- Confirm the password is correct.
- Ask for the exact error message.
- Ask when the issue started.
- Test the Login API.
- Review the HTTP status code returned.

### Possible Outcomes

**200 OK**

The login request worked successfully.

**Support Action**

Investigate browser, cache, or device issues.

---

**401 Unauthorized**

Customer authentication failed.

**Support Action**

Recommend resetting the password or confirming login credentials.

---

**500 Internal Server Error**

Server failure.

**Support Action**

Collect evidence and escalate to Engineering.

---

# Example 2 – Password Reset Email Not Received

### Customer Report

> "I never received my password reset email."

### Investigation Checklist

- Verify the customer's email address.
- Ask the customer to check Spam or Junk folders.
- Confirm the password reset request was submitted.
- Test the Password Reset API.
- Check email service availability.

### Possible Outcomes

API returns **200 OK**

The email request was accepted.

Support should verify customer email information.

---

API returns **500 Internal Server Error**

The email service failed.

Escalate to Engineering.

---

# Information to Collect Before Escalating

Always include:

- Customer ID or Email
- Date and Time issue occurred
- Error message
- Screenshots
- Steps to reproduce
- API response
- HTTP status code
- Business impact

Providing complete information helps Engineering investigate issues faster.

---

# Best Practices

✔ Ask questions before making assumptions.

✔ Reproduce the issue whenever possible.

✔ Check API responses before escalating.

✔ Document every investigation clearly.

✔ Keep customers informed throughout the troubleshooting process.

---

# Key Takeaways

✔ API troubleshooting helps identify the root cause of customer issues.

✔ HTTP status codes guide troubleshooting decisions.

✔ Product Support Engineers gather evidence before escalating.

✔ Good troubleshooting reduces unnecessary Engineering escalations.

---

**Next:** [04-Postman-Basics.md](./04-Postman-Basics.md)
