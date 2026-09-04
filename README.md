# Laundry Pickup System.

A software engineering project: full requirements analysis, system design, and architecture for a laundry pickup and delivery platform connecting customers, laundry staff, and an external delivery provider.

## Overview

The Laundry Pickup System allows customers to schedule laundry pickup and delivery, choose services, pay online, and track order status in real time. Laundry staff manage orders, pricing, and delivery coordination through the same platform. The system was designed using the **Agile development model**, delivered in iterative stages (account management, ordering, tracking, payment, delivery, reporting).

## My Contribution

This was a 4-member team project. I was responsible for:

- **System Requirements** — translated user-level functional requirements into detailed system-level specifications (14 requirement groups covering account management, ordering, payment, delivery coordination, and reporting)
- **Non-Functional Requirements** — defined measurable targets for:
  - **Security:** AES-256 encryption for all customer/driver/laundry data, OTP or email-based authentication, role-based access control (RBAC)
  - **Scalability:** support for 1,500+ concurrent users, with headroom for future laundries and drivers
  - **Availability:** 99.9% uptime, automatic failover to backup servers, database backups every 12 hours
  - **Cross-platform support:** Flutter (front-end) and Node.js (back-end), tested across 3+ browser versions and 5+ screen resolutions
- **Context Diagram** — modeled the system's boundary and its integration with Authentication, Payment Gateway, Delivery Provider, and Location Maps services
- **Use-Case Scenarios** — wrote full Main Success Scenarios and extensions for *Manage Services & Pricing*, *View & Manage Customer Orders*, *Manage Delivery Process*, and *Generate Reports*
- **Class Diagram** — fully reviewed and refined the system's class structure (Customer, Order, Service, Payment, DeliveryService, Feedback, LaundryStaff)
- **Activity Diagram** — designed the flow for *Pay via External Payment System*
- **System Architecture** — selected and documented a **Client-Server Architecture**, chosen for clear separation between client interface and server logic, centralized security, easier maintenance, and scalability

## Architecture

Client-Server model with four core services behind a shared internet layer: **Authentication Service**, **Laundry Management Service**, **Payment Service**, and **Database** — accessed by Staff, Customers, and the Delivery Provider.

## Tech Stack

Flutter (front-end) · Node.js (back-end) · Agile methodology · UML (Use-Case, Class, Sequence, Activity, State diagrams)
