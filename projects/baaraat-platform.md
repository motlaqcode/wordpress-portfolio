# Baaraat — WordPress Publishing & Support Automation Platform

[← Back to portfolio](../README.md)

<small>Private backend project · Public website and WordPress plugin</small>

## Overview

Baaraat is a platform designed to connect a Telegram-based workflow with WordPress websites, helping users initiate and manage content-publishing tasks through a conversational interface.

The platform uses a central backend and a site-side WordPress agent to coordinate work between the Telegram experience and connected WordPress installations. The project includes workflows for product and article publishing, site pairing, job processing, and subscription-related operations.

## Project Links

- **Official website:** [baaraat.ir](https://baaraat.ir/)
- **WordPress plugin:** [Baaraat Agent on WordPress.org](https://fa.wordpress.org/plugins/baaraat-agent/)
- **Telegram bot:** [@baaraatBot](https://t.me/baaraatBot)

## My Role

**Backend Developer & Technical Lead**

I designed, implemented, and maintained core application workflows, backend services, WordPress connectivity, and operational behavior.

## Technology

- **Backend:** Python
- **API framework:** FastAPI
- **Application interface:** Telegram Bot API
- **WordPress integration:** Custom site-side agent/plugin and WordPress REST/API workflows
- **Data layer:** SQLite
- **Deployment:** Linux, Docker, Uvicorn

## Selected Engineering Work

### Telegram-driven publishing workflows

Built conversational workflows for initiating product and article publishing tasks and guiding users through the process.

- Product and article content workflows
- Progress and completion feedback
- Handling concurrent content operations
- Returning publishing results to the user

### WordPress site connection and agent lifecycle

Implemented the connection flow between the platform and individual WordPress sites.

- Site pairing and registration
- Support for managing multiple connected sites and switching between them
- Site status tracking
- Controlled disconnect and recovery behavior

### Asynchronous job processing

Designed a job-based communication flow between the backend and connected WordPress agents.

- Creating and tracking publishing jobs
- Targeted job claiming by the connected site agent
- Job completion and failure reporting
- Lease-based job claiming to reduce duplicate processing
- Payload size limits and validation

### Request authentication and security

Worked on securing communication between the central service and connected WordPress agents.

- Signed agent requests
- Request nonce handling and replay protection
- Request-body hashing
- Signature-version migration and enforcement
- Authenticated site lifecycle operations

### Subscription and payment workflows

Implemented backend components for subscription and payment-related operations, including payment initiation and callback handling.

## Engineering Priorities

- Keep communication between the backend and WordPress sites authenticated
- Make job execution traceable and resilient to failed requests
- Handle site connection and disconnection as explicit lifecycle events
- Validate request payloads and apply size limits
- Keep private service logic and deployment configuration out of public documentation

## Project Access

The central backend repository and internal implementation remain private. The WordPress plugin is publicly available through the official WordPress.org plugin directory. This case study describes selected capabilities and engineering work without exposing credentials, customer data, or private deployment details.
