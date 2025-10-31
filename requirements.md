# Backend Requirements Specification – Airbnb Clone

## 1. User Authentication

### Endpoints

- **POST /api/auth/register** – Create new account
- **POST /api/auth/login** – Authenticate and issue JWT
- **GET /api/auth/profile** – Retrieve user details (Auth required)

### Validation

- Email must be unique and valid.
- Password min length: 8 chars, hashed using bcrypt.

### Response

- JSON containing `accessToken`, `userId`, and `role`.

---

## 2. Property Management

### Endpoints

- **POST /api/properties** – Add new property (Host only)
- **GET /api/properties** – Retrieve all listings
- **PUT /api/properties/:id** – Update property details
- **DELETE /api/properties/:id** – Remove property

### Validation

- Required fields: `title`, `price`, `location`.
- Image uploads via cloud storage (e.g., Cloudinary).

---

## 3. Booking System

### Endpoints

- **POST /api/bookings** – Create new booking
- **GET /api/bookings/:id** – Retrieve booking details
- **DELETE /api/bookings/:id** – Cancel booking

### Process Flow

1. Guest searches available listings.
2. System checks availability.
3. Booking record created.
4. Payment initiated.

### Output

- Confirmation message + booking reference.

---

## Non-Functional Requirements

- **Performance:** Response time < 1s for 95% of requests.
- **Security:** JWT-based authentication, password hashing.
- **Scalability:** Designed for distributed architecture.
- **Reliability:** Database transactions ensure data consistency.
