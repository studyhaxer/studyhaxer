# Hi, I'm Hafiz Atta Ur Rahman 👋

🎓 M.Phil in Computer Science (Gold Medalist)  
Former PHP & WordPress developer rebuilding from scratch with Python.  
One project a day. Everything documented publicly.

---

## 🚀 The Challenge

**#60DaysOfPython** — Started from zero, building one real project every single day.  
Currently on **Day 20** — kicking off the flagship capstone.

🔗 **Live API (Day 19):** [day19-deployment-production.up.railway.app/docs](https://day19-deployment-production.up.railway.app/docs) — deployed FastAPI + Postgres, tested end-to-end against a real production database.

🎓 **Capstone in progress:** [AI-Powered Educational Platform](https://github.com/studyhaxer/capstone-edu-platform) — FastAPI + PostgreSQL + JWT auth + OpenAI-generated lesson summaries & quizzes + React frontend, deploying to **usachunian.com**. Full Day 20–36 roadmap in the repo README.

---

## 🛣️ Journey So Far

| Phase | Days | What I Learned |
|-------|------|----------------|
| Python Core | 1–6 | Basics, CLI, file handling, OOP, JSON/CSV, logging, modular architecture |
| OOP Deep Dive | 7–9 | Encapsulation, `@property`, inheritance, polymorphism |
| Database | 10 | SQLite, CRUD, multi-file structure |
| FastAPI | 11–13 | REST API, Pydantic, SQLAlchemy ORM, `Depends()`, search & filters |
| Relationships | 14 | One-to-Many, cascade delete, `joinedload`, nested Pydantic schemas |
| Auth | 15–17 | JWT (python-jose), bcrypt hashing, OAuth2PasswordBearer, protected routes, RBAC, reusable dependency factories, multi-role routes, dependency composition |
| Testing | 18 | pytest, TestClient, custom exception classes, isolated test DB with autouse fixtures, role-based test coverage, permission-before-fetch pattern |
| Deployment | 19 | Production deployment — managed Postgres (Supabase), env-based secrets, Railway hosting, dynamic port binding, end-to-end verification against a live database |
| **Capstone (in progress)** | **20–36** | **AI-Powered Educational Platform — FastAPI + PostgreSQL + JWT auth, OpenAI lesson summaries & MCQ quiz generation, React frontend, deploying to usachunian.com. [Full roadmap →](https://github.com/studyhaxer/capstone-edu-platform)** |

<details>
<summary>📋 Day-by-day breakdown</summary>

| Day | Project | What I Learned |
|-----|---------|----------------|
| 1–6 | Student Grade Analyzer (v1–v7) | Python basics, CLI, file handling, OOP, JSON/CSV, logging, validation, modular architecture |
| 7–9 | Bank System & Library Management System | Encapsulation, `@property`, deposit/withdraw, inheritance, polymorphism, base class design |
| 10 | Student Management System | SQLite, CRUD, multi-file structure |
| 11–13 | FastAPI APIs (Notes & SQLite) | REST routes, Pydantic models, full CRUD, SQLAlchemy ORM, `Depends()`, `response_model`, keyword search & filters |
| 14 | User Course API | One-to-Many relationships, cascade delete, `joinedload`, nested schemas |
| 15 | JWT Authentication API | JWT (python-jose), bcrypt password hashing, OAuth2PasswordBearer, protected routes via `Depends()` |
| 16 | Role-Based API | Role field on the User model, role-gated routes via dependency factories (`require_role`, `require_any_role`), reusable `pagination_params` dependency, deliberate 401-vs-403 design, `SECRET_KEY` moved to environment variable |
| 17 | Reusable Auth & Role Dependencies | Refactored Day 16's inline role checks into a single reusable `require_any_role` dependency factory; `get_current_user` fully isolated as a standalone dependency; added a "any logged-in user" route (`/me`) and a multi-role route (`/dashboard`); combined `get_db` + role dependency in the same route |
| 18 | FastAPI Testing + Cleanup | pytest suite with TestClient, conftest fixtures with autouse reset_db (clean DB per test), isolated test database, custom exception classes (ForbiddenException, NotFoundException), consistent permission-before-fetch pattern across endpoints, role-based test coverage (401 / 403 / 200 scenarios) |
| 19 | Production Deployment | Swapped SQLite for managed Supabase Postgres; moved `SECRET_KEY` and `DATABASE_URL` fully into platform env vars; fixed Uvicorn start command for dynamic `$PORT` + `0.0.0.0` binding; deployed to Railway; verified full request lifecycle (register → login → protected routes) against the live database, not just that the server started |
| **20** | **Capstone Kickoff — AI-Powered Educational Platform** | **Designed 4-table schema (`User`, `Course`, `Lesson`, `Enrollment`) with a proper many-to-many `Enrollment` bridge model, `UniqueConstraint` to prevent duplicate enrollments, `NOT NULL` foreign keys; Pydantic schemas with nested `List[LessonOut]`; resolved a production-grade Supabase IPv6/DNS issue by switching to the session pooler connection string; verified all tables live in Supabase and pushed to a dedicated capstone repo** |

</details>

> 📋 Days 20–36 of the capstone follow a detailed phase-by-phase roadmap (auth → CRUD → AI features → React frontend → deployment) — see the [capstone repo README](https://github.com/studyhaxer/capstone-edu-platform) for the full breakdown.

---

## 🧰 Tech Stack

- **Language:** Python 3
- **Backend:** FastAPI, Uvicorn
- **Database:** PostgreSQL (Supabase, production), SQLite (local dev), SQLAlchemy ORM
- **Auth:** JWT, bcrypt, python-jose, passlib
- **Testing:** pytest, httpx, TestClient
- **Deployment:** Railway, Supabase, environment-based secrets management
- **Concepts:** OOP, REST API, CRUD, Pydantic v2, DB Relationships, Role-Based Access Control, Reusable Dependencies, Testing, Production Deployment, File Handling, Logging

---

## 📌 Featured Projects

- 🎓 [**AI-Powered Educational Platform**](https://github.com/studyhaxer/capstone-edu-platform) — *60-day capstone, in progress.* FastAPI + PostgreSQL + JWT auth, OpenAI lesson summaries & MCQ quiz generation, React frontend, deploying to usachunian.com
- 🚀 [Production Deployment](https://github.com/studyhaxer/day19-deployment) — FastAPI live on Railway, Supabase Postgres, env-based secrets, full request lifecycle verified end-to-end
- 🧪 [FastAPI Testing + Cleanup](https://github.com/studyhaxer/day18-testing-cleanup) — pytest suite, TestClient, isolated test DB, custom exception classes, role-based test coverage
- 🔁 [Reusable Auth & Role Dependencies](https://github.com/studyhaxer/day17-reusable-auth-dependencies) — JWT auth and RBAC fully moved into reusable dependency functions, multi-role routes, dependency composition
- 🔑 [Role-Based API](https://github.com/studyhaxer/day16-role-based-api) — RBAC with `require_role`/`require_any_role` dependency factories, reusable pagination dependency, 401 vs 403 design
- 🔐 [JWT Authentication API](https://github.com/studyhaxer/day15-jwt-auth-api) — JWT auth, bcrypt password hashing, protected routes with OAuth2
- 🔗 [User Course API](https://github.com/studyhaxer/day14-user-course-api) — One-to-Many relationships, cascade delete, nested Pydantic schemas
- 🗒️ [FastAPI SQLite API](https://github.com/studyhaxer/python-day13-fastapi-sqlite-api) — SQLAlchemy ORM, keyword search, filters, response_model
- 🗒️ [FastAPI Notes API](https://github.com/studyhaxer/python-day12-fastapi-notes-api) — Full CRUD REST API with Pydantic models
- 🎓 [Student Management System](https://github.com/studyhaxer/student-management-system-v1) — SQLite + Python CLI with full CRUD
- 📚 [Library Management System](https://github.com/studyhaxer/library-management-system-v1) — OOP with inheritance and polymorphism
- 🏦 [Bank System](https://github.com/studyhaxer/bank-system-v1) — OOP with `@property` and transaction history

---

## 📈 Background

- 🏢 Former PHP Developer & WordPress Developer
- 🌐 REST API experience from Elance/Odesk freelancing
- 🎯 Goal: Return to professional software development within 90 days
- 📍 Based in Lahore, Pakistan

---

## 🔗 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-studyhaxer-blue?style=flat&logo=linkedin)](https://linkedin.com/in/studyhaxer)
[![Twitter](https://img.shields.io/badge/Twitter-@hafizzatta-1DA1F2?style=flat&logo=twitter)](https://twitter.com/hafizzatta)
[![GitHub](https://img.shields.io/badge/GitHub-studyhaxer-black?style=flat&logo=github)](https://github.com/studyhaxer)

---

> "One project a day. No shortcuts. No breaks." 🐍
