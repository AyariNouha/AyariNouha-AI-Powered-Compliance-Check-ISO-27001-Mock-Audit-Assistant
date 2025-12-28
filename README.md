# AI-Powered Compliance Check: ISO 27001 Mock Audit Assistant
Python Django • Next.js  • PostgreSQL • Docker • License

Web-based platform for simulating ISO 27001 compliance audits with AI-powered analysis, automated reporting, and intelligent dashboards.

Demo • Documentation • Installation

🎯 Features
🤖 AI Integration: Mistral LLM for intelligent audit analysis & recommendations

📊 Interactive Dashboard: Real-time compliance status & audit progress visualization

🚨 Smart Alerts: Automatic detection of non-conformities before official audits

📝 Audit Workflow: Clause management, audit scheduling, and feedback collection

📂 Automated Reports: Export audit results in structured formats (PDF, JSON)

🐳 Docker Ready: One-command deployment for frontend + backend

🔒 Security First: JWT authentication, RBAC, and environment-based configuration

🏗️ Architecture
Code
┌─────────────┐      ┌──────────────┐      ┌─────────────┐
│   Frontend  │─────▶│   Backend    │─────▶│   AI Engine │
│  (Next.js)  │      │   (Django)   │      │ (Mistral LLM)│
└─────────────┘      └──────────────┘      └─────────────┘
       │                     │                      │
       └─────────────▶ PostgreSQL ◀─────────────────┘
                            │
                       Redis (Celery)
🚀 Quick Start
Prerequisites
Docker & Docker Compose

Git

Installation
bash
# Clone repository
git clone https://github.com/AyariNouha/AI-Powered-Compliance-Check-ISO-27001-Mock-Audit-Assistant
cd iso27001-compliance-ai



# Access dashboard
open http://localhost:3000
🎉 That’s it!

💻 Tech Stack
Backend
Framework: Django 4.2 + Django REST Framework

Database: PostgreSQL 15

Task Queue: Celery + Redis

Auth: JWT + RBAC

AI Engine
Model: Mistral LLM

Libraries: Transformers, LangChain, Pandas, NumPy

Use Cases: Audit question analysis, scoring, compliance recommendations

Frontend
Framework: Next.js  14 + TypeScript

UI: Tailwind CSS + Recharts

State: React Query (TanStack)

DevOps
Containerization: Docker + Docker Compose

CI/CD: GitHub Actions (optionnel)

📖 Documentation
API Endpoints
Code
GET  /api/users/          # User management
GET  /api/audits/         # List audits
POST /api/audits/plan     # Schedule mock audit
GET  /api/audits/results  # Audit results & scores
POST /api/feedback/       # Submit feedback
Environment Variables
bash
# Backend (.env)
DB_NAME=iso27001db
DB_USER=iso27001user
DB_PASSWORD=your_password
SECRET_KEY=your_secret_key
REDIS_URL=redis://redis:6379/0

# Frontend (.env.local)
NEXT_PUBLIC_API_URL=http://localhost:8000/api
NEXT_PUBLIC_WS_URL=ws://localhost:8001/ws
🙏 Acknowledgments
VERMEG Factory for hosting the internship

Django & Next.js  communities

Open-source AI libraries (Mistral, HuggingFace, LangChain)

ISO/IEC 27001 standard documentation

⭐ Star this repo if you find it helpful!

Made with ❤️ by Nouha Ayari
