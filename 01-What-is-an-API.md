# What is an API?

## Introduction

As a Product Support Engineer, you don't need to build APIs, but you do need to understand how they work. APIs help you investigate customer issues, communicate with Engineering teams, and troubleshoot problems more effectively.

---

## What is an API?

API stands for **Application Programming Interface**.

An API acts as a messenger between an application and a server. When a user performs an action in an app, the API sends the request to the server and returns the server's response back to the application.

In simple terms:

> **The API allows different software systems to communicate with each other.**

---

## How APIs Work

Imagine a customer is using a banking app.

The customer enters their email and password and clicks **Login**.

The process looks like this:

Customer

↓

Mobile App

↓

API Request

↓

Server

↓

API Response

↓

Mobile App

↓

Customer

The customer never sees the API, but it is responsible for carrying the request and the response between the app and the server.

---

## API Example from a Product Support Perspective

### Customer Issue

> "I can't log into my account."

Instead of immediately escalating the issue, a Product Support Engineer investigates.

Possible checks include:

- Is the login service available?
- Is the API responding?
- What HTTP status code is being returned?
- Is this affecting one customer or multiple customers?

If the Login API returns:

- **200 OK** → The request worked successfully.
- **401 Unauthorized** → The customer's login credentials are incorrect.
- **500 Internal Server Error** → The issue is likely on the server and should be escalated to Engineering.

Understanding API responses helps Product Support Engineers identify the source of a problem more quickly.

---

## Why APIs Matter in Product Support

Understanding APIs helps Product Support Engineers:

- Troubleshoot customer issues more efficiently.
- Determine whether an issue is caused by the customer or the system.
- Communicate technical findings to Engineering teams.
- Reduce unnecessary escalations.
- Improve customer experience by identifying issues faster.

---

## Real-World Example

Customer reports:

> "My password reset email never arrived."

Possible investigation:

- Confirm the customer's email address.
- Check whether the Password Reset API responded successfully.
- Verify whether the email service is operational.
- Escalate only if the API or email service is failing.

---

## Key Takeaways

✔ API stands for Application Programming Interface.

✔ APIs allow applications and servers to communicate.

✔ Product Support Engineers use APIs to investigate customer issues.

✔ API responses help determine whether a problem is customer-related or server-related.

✔ Understanding APIs improves troubleshooting and communication with Engineering teams.

**Next:** [02-HTTP-Status-Codes.md](./02-HTTP-Status-Codes.md)
