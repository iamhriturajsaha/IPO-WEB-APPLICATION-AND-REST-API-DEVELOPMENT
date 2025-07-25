# 🌐IPO Web Application and REST API Development

## 🧾 Project Overview

This project is developed as part of the Bluestock Fintech Internship Program and focuses on building a **production-grade full-stack IPO Web Application**. It includes -

- A **client-facing IPO listing module** (Upcoming IPO Web Page)
- A complete **Admin Dashboard** for IPO management
- A secure and scalable **REST API backend**
- **JWT-based authentication**
- **PostgreSQL** as the primary database

This solution is suitable for integration into stock market platforms, IPO tracking apps or client-side fintech tools.

---

## ⚙️ Tech Stack

| Layer         | Technology                         |
|--------------|-------------------------------------|
| Frontend     | ReactJS or Angular                  |
| Backend      | Django / NodeJS / Spring Boot       |
| Database     | PostgreSQL                          |
| API Protocol | REST (Tested via Postman)           |
| Auth         | JWT-based Authentication            |
| Dev Tools    | VS Code, GitHub, Chrome DevTools    |
| Styling      | TailwindCSS / SCSS, Prettier, ESLint|

---

## 🚀 Key Modules

### 1. Upcoming IPO Webpage (User-Facing)

- Standalone module for displaying upcoming IPOs.
- Uses REST API to fetch data dynamically.
- Displays IPOs in a card/grid layout with -
  - Company Name
  - Price Band
  - IPO Open/Close Dates
  - Lot Size
  - Issue Size
  - Listing Date
  - Status Tags (Upcoming / Ongoing / Closed / Listed)
- Includes search, filters (by date, sector), pagination.
- Fully responsive across desktop, tablet and mobile.
- Pixel-perfect UI based on Figma design.

### 2. IPO Admin Dashboard

- Admin login with static form validation + JWT token.
- CRUD operations on IPO data -
  - Add new IPO
  - Edit existing IPO
  - Delete IPO
- Interactive form with validation and real-time feedback.
- Admin Dashboard Table with search/sort.
- Data directly synced with backend via REST API.
- Protected routes (JWT-secured) for sensitive operations.

### 3. REST API Backend

- Implemented using Django / NodeJS / Spring Boot.
- Built using modular MVC or similar clean architecture.
- JWT token-based authentication.
- PostgreSQL database integration with schema & seed data.
- API documentation and testing done via Postman.
- Handles -
  - User login & token issuance
  - IPO data CRUD
  - Validation, error handling & auth middleware

---

## 🔐 Authentication & Authorization

- **JWT-based** token system for admin login.
- Login route returns token on success.
- Tokens stored in localStorage/sessionStorage in frontend.
- Protected backend routes require JWT in `Authorization` header.
- Middleware handles unauthorized access with 401 errors.

---

## 🧪 API Endpoints Overview

| Method | Endpoint            | Description                  | Auth |
|--------|---------------------|------------------------------|------|
| POST   | `/api/login`        | Admin login (JWT token)      | ✅  |
| GET    | `/api/ipos`         | Get all IPOs                 | ✅  |
| GET    | `/api/ipos/:id`     | Get IPO by ID                | ✅  |
| POST   | `/api/ipos`         | Add new IPO                  | ✅  |
| PUT    | `/api/ipos/:id`     | Update IPO                   | ✅  |
| DELETE | `/api/ipos/:id`     | Delete IPO                   | ✅  |

---

## 🧪 API Testing (Postman)

All REST APIs have been tested in Postman with authentication headers and payload validation.

- Admin login generates token.
- CRUD endpoints tested with valid/invalid tokens.
- Backend handles -
  - Validation errors (400)
  - Unauthorized access (401)
  - Success responses (200/201)
  - Resource not found (404)

---

## ✅ Tasks Completed

| No.| Task Name                               | Description                                                               |
|----|-----------------------------------------|---------------------------------------------------------------------------|
| 1  | Alpha Testing                           | Final phase execution and QA validation.                                  |
| 2  | API Testing in Postman                  | All endpoints tested for success, failure, auth, and validations.         |
| 3  | Backend Development                     | REST API implemented using Django/Node/Spring Boot. JWT secured.          |
| 4  | Bug Fixing                              | Fixed minor debugging in UI and API integration.                          |
| 5  | Database Design & Dummy Data Population | PostgreSQL schema created, data seeded with representative IPO entries.   |
| 6  | Deployment Prep & Technical Docs        | README and Postman export prepared; production build generation underway. |
| 7  | Frontend (React/Angular)                | Upcoming IPO Web Page and Admin Dashboard UI completed.                   |
| 8  | Prerequisite Setup                      | All environment tools (Node, Python, DB, etc.) installed and verified.    |
| 9  | Environment Configuration               | .env files created, all frameworks/libraries installed and configured.    |
| 10 | REST API Development & JWT              | Backend routes secured and JWT authentication system operational.         |
| 11 | Upcoming IPO UI Design                  | Fully responsive, Figma-matched, production-grade UI implemented.         |
