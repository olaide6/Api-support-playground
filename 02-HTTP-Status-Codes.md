# HTTP Status Codes

## Introduction

Whenever an application sends an API request, the server responds with an HTTP status code.

These status codes tell Product Support Engineers whether the request was successful or if something went wrong.

Understanding HTTP status codes helps support teams troubleshoot customer issues more efficiently and determine whether an issue should be escalated.

---

# Common HTTP Status Codes

| Status Code | Meaning | What it Means for Product Support |
|-------------|---------|-----------------------------------|
| **200 OK** | Request successful | The API worked successfully. The issue may be related to user input or another part of the application. |
| **201 Created** | Resource successfully created | A new account, record, or resource was created successfully. |
| **400 Bad Request** | Invalid request | The request contains invalid or missing information. Ask the customer to verify their input. |
| **401 Unauthorized** | Authentication failed | The customer is not authenticated. Ask them to log in again or reset their password. |
| **403 Forbidden** | Permission denied | The customer is logged in but does not have permission to access the requested resource. |
| **404 Not Found** | Resource not found | The requested page, account, or resource cannot be found. Verify the URL or account details. |
| **429 Too Many Requests** | Rate limit exceeded | Too many requests were sent in a short period. Ask the customer to wait and try again later. |
| **500 Internal Server Error** | Server error | Something went wrong on the server. Escalate the issue if it persists. |
| **502 Bad Gateway** | Server communication issue | One server received an invalid response from another server. Usually requires Engineering investigation. |
| **503 Service Unavailable** | Service temporarily unavailable | The service is down or under maintenance. Inform the customer and monitor service restoration. |

---

# Real Product Support Example

### Customer Issue

> "I can't update my profile."

Investigation:

The API returns:

**403 Forbidden**

Interpretation:

The customer is logged in successfully, but their account does not have permission to perform the requested action.

Support Action:

- Verify the customer's account permissions.
- Confirm their subscription or user role.
- Escalate if permissions appear correct but the issue persists.

---

# When Should You Escalate?

Generally, Product Support can investigate many **4xx** errors by working with the customer.

**5xx** errors usually indicate server-side problems and may require escalation to Engineering after gathering enough information.

Before escalating:

- Collect screenshots.
- Record the time the issue occurred.
- Identify the affected user(s).
- Document the API response.
- Include reproduction steps.

---

# Key Takeaways

✔ HTTP status codes describe the result of an API request.

✔ 2xx status codes indicate successful requests.

✔ 4xx status codes usually relate to customer requests or permissions.

✔ 5xx status codes usually indicate server-side problems.

✔ Understanding status codes helps Product Support troubleshoot and escalate issues effectively.

---

**Next:** [03-API-Troubleshooting.md](./03-API-Troubleshooting.md)
