# Airbnb Clone Backend - Features and Functionalities

## Overview

This document outlines the key backend features and functionalities required for the Airbnb Clone system. The backend provides APIs for user management, property listings, bookings, payments, and reviews.

---

## 1. User Management

- User registration and login (JWT-based authentication)
- Password encryption (bcrypt)
- Role-based access (guest, host, admin)
- Profile management (view/update user info)

---

## 2. Property Management

- Hosts can add, edit, or delete property listings
- Upload property details: name, description, location, price per night
- Retrieve available listings with search and filtering

---

## 3. Booking System

- Guests can book available properties
- Prevent overlapping bookings
- Hosts can approve or reject booking requests
- Booking statuses: pending, confirmed, canceled

---

## 4. Payment Processing

- Integration with Stripe/PayPal
- Handle booking payments securely
- Payment receipts and transaction history

---

## 5. Reviews and Ratings

- Guests can review properties after their stay
- Ratings between 1–5 stars
- Reviews linked to users and properties

---

## 6. Messaging System

- Direct communication between guests and hosts
- Messages stored per conversation thread

---

## 7. Admin Management

- Admin can manage users, properties, and bookings
- Monitor system analytics and resolve disputes

---

## 8. System Features

- Secure JWT authentication
- RESTful API architecture
- PostgreSQL database with relational mapping
- Error handling and input validation
