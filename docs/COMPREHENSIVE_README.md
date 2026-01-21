# Research Notebook – Comprehensive README

Welcome to the Research Notebook project! This document provides a detailed overview of the system, its features, and direct links to the relevant code files for easy navigation.

---

## Table of Contents
- [Project Overview](#project-overview)
- [API Endpoints](#api-endpoints)
  - [Authentication](#authentication)
  - [User Management](#user-management)
  - [Contacts & Requests](#contacts--requests)
  - [Direct Messages & Mentions](#direct-messages--mentions)
  - [Notes & Projects](#notes--projects)
  - [Todos & Templates](#todos--templates)
  - [Uploads](#uploads)
  - [Webhooks & Real-time](#webhooks--real-time)
  - [Debug & Health](#debug--health)
- [Core Libraries](#core-libraries)
- [Frontend](#frontend)
- [Testing](#testing)
- [Scripts](#scripts)
- [Deployment](#deployment)
- [Documentation](#documentation)
- [Known Issues](#known-issues)

---

## Project Overview
This project is a full-stack research notebook and collaboration platform. It features RESTful APIs, authentication, real-time updates, file uploads, and a static HTML frontend. MongoDB is used for data storage, and the project is designed for deployment on Vercel.

---

## API Endpoints
All API endpoints are located in the [api/](api) directory.

### Authentication
- [Register](api/auth/register.js): User registration
- [Login](api/auth/login.js): User login
- [Logout](api/auth/logout.js): User logout
- [Me](api/auth/me.js): Get current user info
- [Change Password](api/auth/change-password.js): Change user password
- [Update Profile](api/auth/update-profile.js): Update user profile

### User Management
- [Users](api/users.js): List, search, and manage users

### Contacts & Requests
- [Contacts](api/contacts.js): Manage user contacts
- [Contact Requests](api/contact_requests.js): Handle contact requests
- [Invitations](api/invitations.js): Manage invitations

### Direct Messages & Mentions
- [Direct Messages](api/direct-messages.js): Send and receive direct messages
- [Mentions](api/mentions.js): Mention users in notes/messages

### Notes & Projects
- [Notes](api/notes.js): Create, edit, and manage notes
- [Projects](api/projects.js): Manage projects
- [Project Notes](public/project-notes.html): Project-specific notes (frontend)

### Todos & Templates
- [Todos](api/todos.js): Manage todo items
- [Templates](api/templates.js): Note and project templates

### Uploads
- [Uploads](api/uploads/images.js): Handle image uploads
- [Image Access](api/uploads/images/[id].js): Access uploaded images

### Webhooks & Real-time
- [Webhook Forwarder](api/webhook-forwarder.js): Forward webhooks to external services
- [Realtime Updates](api/realtime/updates.js): Real-time notifications and updates

### Debug & Health
- [Debug Auth](api/debug-auth.js): Debug authentication
- [Debug Env](api/debug-env.js): Debug environment variables
- [Demo Data](api/demo-data.js): Load demo data
- [Health](api/health.js): Health check endpoint
- [Index](api/index.js): API index/landing
- [Search](api/search.js): Search functionality

---

## Core Libraries
- [Authentication Logic](lib/auth.js)
- [MongoDB Connection](lib/mongo.js)
- [Session Management](lib/sessions.js)
- [Validation Utilities](lib/validate.js)

---

## Frontend
All static frontend files are in the [public/](public) directory:
- [Dashboard](public/dashboard.html)
- [Notes](public/notes.html)
- [Projects](public/projects.html)
- [Contacts](public/contacts.html)
- [Todos](public/todos.html)
- [Login/Register](public/login.html, public/register.html)
- [Profile](public/profile.html)
- [Admin](public/admin.html)
- [Styles](public/styles.css)
- [Client Scripts](public/app.js, public/enhancements.js)

---

## Testing
- [Playwright Config](playwright.config.js): Playwright setup
- [Integration/UI/Visual Tests](tests/):
  - [Example Spec](tests/example.spec.js)
  - [Research Notebook Spec](tests/research-notebook.spec.js)
  - [Visual Regression Spec](tests/visual-regression.spec.js)
- [Test Scripts](scripts/):
  - [Comprehensive Test](scripts/comprehensive-test.js)
  - [Integration Test](scripts/integration-test.js)
  - [UI Flow Tests](scripts/ui-flow-tests.js)
  - [Test Runner](scripts/test.js)
  - [Run Integration Tests](scripts/run-integration-tests.js)

---

## Scripts
- [Seed Database](scripts/seed.js)
- [Add Indexes](scripts/add-indexes.js)

---

## Deployment
- [Vercel Configuration](vercel.json)
- [Build & Run Instructions](BUILD_AND_RUN.md)

---

## Documentation
- [API Reference](docs/API.md)
- [User Guide](docs/USER_GUIDE.md)
- [Implementation Summary](IMPLEMENTATION_SUMMARY.md)
- [Known Issues](KNOWN_ISSUES.md)
- [MongoDB Setup](README-MONGODB.md)
- [Vercel Webhook Setup](README-VERCEL-WEBHOOK.md)

---

## Known Issues
See [KNOWN_ISSUES.md](KNOWN_ISSUES.md) for a list of current issues and limitations.

---

## Contributing
Please see the main [README.md](README.md) for contribution guidelines and project overview.

---

## License
See [README.md](README.md) for license and usage information.

---

For any questions or support, please refer to the [User Guide](docs/USER_GUIDE.md) or open an issue.
