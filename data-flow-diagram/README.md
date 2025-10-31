# Data Flow Diagram (DFD) – Airbnb Clone

## Objective

This document describes how data moves through the Airbnb backend system — from user input to database and response output.

## Levels

- **Level 0 (Context Diagram):** Shows the system as a single process interacting with external entities (Users, Payment Gateway, Database).
- **Level 1 (Detailed DFD):** Breaks the system into modules like Authentication, Booking, and Payments.

## Main Processes

1. User Authentication – Login, Register, Token validation
2. Property Management – CRUD operations on properties
3. Booking System – Availability check, booking creation
4. Payment Handling – Transaction processing, receipts
5. Reviews – Submit and fetch ratings

## Tools

- Draw.io used to design `data-flow.png`
