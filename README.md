# Strent-backend

## 🧾 Project Description
Strent is a secure real estate web and mobile platform that connects homeowners, tenants, and roommates directly. This repository contains the backend codebase for the Strent platform, built using FastAPI, PostgreSQL, and modern backend technologies. It includes user authentication, listing management, messaging, notifications, and secure payment processing.


## 📁 Project Structure
- strent-backend/
- │
- ├── app/
- │   ├── api/                    # Route definitions
- │   ├── core/                   # Settings, config, security
- │   ├── crud/                   # Database interaction logic
- │   ├── db/                     # Database connection and models
- │   ├── schemas/                # Pydantic models (data validation)
- │   ├── models/                 # SQLAlchemy ORM models
- │   ├── services/               # Business logic (auth, messaging, etc.)
- │   └── main.py                 # FastAPI entry point
- │
- ├── alembic/                   # Database migrations
- ├── .env                       # Environment variables
- ├── requirements.txt           # Python dependencies
- ├── Dockerfile                 # Docker container setup
- ├── docker-compose.yml         # Multi-container orchestration
- └── README.md                  # Project info and instructions

## 🛠️ Tech Stack
- FastAPI (Web framework)
- PostgreSQL (Database)
- SQLAlchemy (ORM)
- Alembic (Migrations)
- Pydantic (Data validation)
- JWT / OAuth2 (Authentication)
- Redis (Caching, background tasks)
- Celery (Async tasks, email)
- Socket.IO (Real-time messaging)
- Stripe / Paystack (Payments)
- Docker (Containerization)

## ⚙️ Installation & Local Development
### 📦 Prerequisites
- Python 3.10+
- PostgreSQL
- Docker & Docker Compose

### 🔧 Setup
git clone https://github.com/wendiblac/strent-backend.git
cd strent-backend
cp .env.example .env

### 🐳 Run with Docker
docker-compose up --build

### 🧪 Run Tests
pytest

## 🚀 Deployment
We use AWS EC2 for backend deployment.
- Set up a PostgreSQL database (AWS RDS or equivalent).
- Push your code to main or prod branch.
- Deploy via CI/CD pipeline using GitHub Actions.


## 🧭 Contribution Guidelines
### 🧑‍🤝‍🧑 Who Can Contribute
All backend developers, DevOps engineers, and QA testers.

## 📌 Branch Naming Convention
- feature/<name>     → New features
- doc/<name>         → Documentation
- fix/<name>         → Bug fixes
- refactor/<name>    → Code improvements
- test/<name>        → Test cases

## ✅ How to Contribute
- Fork the repository
- Create a new branch from dev
- Make your changes
- Run tests locally
- Commit changes with descriptive messages
- Create a Pull Request targeting dev
- Request reviews from backend leads

## 🔍 Code Style & Best Practices
- Follow PEP8 coding standards
- Use type hints for all function signatures
- Keep business logic modular
- Use dependency injection for services
- Write tests for all new features
- Avoid committing .env or secrets


## 🧪 Testing
- Use pytest for unit and integration tests
- Test endpoints with Swagger or Postman
- Mock external services in test environment

## 🏗 System Architecture
graph TD
- A[Client (Web/Mobile)] --> B[API Gateway - FastAPI Routes]
- B --> C[Authentication - JWT/OAuth2]
- B --> D[Business Logic - Services Layer
- D --> E[Database - PostgreSQL via SQLAlchemy]
- D --> F[Celery Workers - Async Tasks]
- D --> G[Redis - Caching & Queues]
- D --> H[Payment Gateway - Stripe/Paystack]
- D --> I[Socket.IO - Real-Time Messaging]


## 🔮 Future Backend Enhancements
- Rate Limiting & Throttling
- Admin Dashboard & Analytics
- SMS Verification with Twilio
- Push Notification Service
- API Rate Logs and Monitoring

## 🤝 Contact
For questions, issues, or contributions, please contact the Dev Team Lead or Assistant or raise an issue in the repository, Slack Channel or Whatsapp group.

© 2025 Strent Dev Team. All rights reserved.
