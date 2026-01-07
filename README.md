# Tutor Support System – Frontend

This repository contains the frontend application for the Tutor Support System. This is my project assignment for the Software Engineering course at Ho Chi Minh City University of Technology (HCMUT).

The system is a web-based platform designed to support the management and operation of tutor–student programs in a university environment.

The frontend is built with Next.js and provides role-based user interfaces for students, tutors, and administrators. It communicates with a backend service that handles authentication, business logic, and data validation.

---

## Tech Stack

- **Framework:** Next.js (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **API Communication:** RESTful APIs
- **Authentication:** Cookie-based session handling

---

## User Roles & Responsibilities

The frontend provides separate interfaces tailored to each role:

### Student

- View available courses and class groups
- Register or unregister for classes within allowed timeframes
- View personal schedules and session information
- Submit feedback and evaluations

### Tutor
- View assigned classes and enrolled students
- Manage class schedules and sessions
- Track attendance and learning progress
- Review feedback related to their courses

### Administrator
- Manage course and class configurations
- Assign tutors to classes
- Monitor system usage and participation
- Access aggregated reports and statistics

## Key Features
- Role-based dashboards and navigation
- Course and class registration interfaces
- Tutor scheduling and session management views
- Feedback and evaluation submission forms
- Reporting and data visualization pages
- Secure authentication using cookie-based sessions

## Frontend Architecture

The frontend is organized around **domain features** rather than individual pages. This structure improves maintainability and mirrors backend concepts such as courses, registrations, scheduling, feedback, and reporting.

Key architectural principles:
- Clear separation between UI components and API logic
- Feature-based organization for scalability
- Minimal business logic in the frontend
- Backend as the single source of truth
---

## Getting Started

### Prerequisites
- Node.js (v18 or later)
- npm

### Installation

Install dependencies:
```bash
npm install
```

Run the development server:
```bash
npm run dev
```

Open your browser and navigate to:
```bash
http://localhost:3000
```

### Environment Configuration

This project requires environment variables for API endpoints and authentication settings.

Create a .env.local file based on the provided example:
```bash
cp .env.example .env.local
```

Fill in the required values before running the application.

### Authentication Notes

For security reasons, no real or hardcoded user credentials are included in this repository.

Authentication depends on the backend service and its configured user accounts.

### Related Repositories

Backend service: [Tutor Support System – Backend](https://github.com/phatpinkkk/tutor-support-system-backend)

### License

This project is intended for educational and demonstration purposes.
