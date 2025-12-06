# NXTRIX - Creative Finance Deal Analyzer & CRM

[![License](https://img.shields.io/badge/license-Proprietary-red.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.11+-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/streamlit-1.28+-FF4B4B.svg)](https://streamlit.io)
[![PostgreSQL](https://img.shields.io/badge/postgresql-15+-336791.svg)](https://postgresql.org)

<p align="center">
  <img src="attached_assets/generated_images/nxtrix_premium_purple-blue_logo.png" alt="NXTRIX Logo" width="200">
</p>

<p align="center">
  <strong>The ultimate deal analysis platform built specifically for creative finance real estate investors.</strong>
</p>

<p align="center">
  <a href="https://nxtrix.com">Website</a> •
  <a href="#features">Features</a> •
  <a href="#pricing">Pricing</a> •
  <a href="#tech-stack">Tech Stack</a>
</p>

---

## Overview

NXTRIX helps wholesalers, flippers, BRRRR investors, and creative finance specialists analyze deals in **60 seconds instead of 60 minutes** - with Monte Carlo simulation, AI-powered deal scoring, and a full CRM to manage your pipeline from lead to close.

**Stop losing money to spreadsheet errors. Analyze deals the right way.**

---

## Features

### Deal Analysis Tools
| Tool | Description |
|------|-------------|
| **MAO Calculator** | Maximum Allowable Offer for wholesale, flip, and rental strategies |
| **Fix & Flip Analysis** | Complete profit projections with holding costs and timeline |
| **BRRRR Calculator** | Buy, Rehab, Rent, Refinance, Repeat with cash-on-cash returns |
| **Subject-To Analysis** | Full creative finance deal modeling with equity capture |
| **Owner Finance Calculator** | Seller financing scenario analysis and amortization |
| **Lease Option Analysis** | Rent-to-own deal structuring and projections |
| **Monte Carlo Simulation** | Run 1,000+ scenarios to stress-test your deals |
| **AI Deal Scoring** | Automated deal quality assessment (0-100 score) |

### CRM & Pipeline Management
- **Contact Management** - Track leads, sellers, buyers, and investors with custom fields
- **Deal Pipeline** - Kanban-style deal tracking from lead to close
- **Activity Logging** - Complete interaction history with timestamps
- **Task Management** - Never miss a follow-up with automated reminders
- **Lead Scoring** - Prioritize your hottest opportunities

### Automation & Communication
- **Email Integration** - SendGrid-powered transactional emails and templates
- **SMS Notifications** - Twilio-powered text messaging and alerts
- **Drip Campaigns** - Automated follow-up sequences that run 24/7
- **Calendar Integration** - Google Calendar sync for appointments
- **Direct Messaging** - Send emails and texts directly from contact profiles

### Portfolio & Investor Management
- **Portfolio Analytics** - Track your holdings, equity, and cash flow
- **Investor Portal** - Manage investor relationships and capital commitments
- **Deal Matching** - Auto-match deals with investor criteria
- **Performance Reports** - ROI tracking across your portfolio

### Enterprise Features
- **Team Collaboration** - Multi-seat plans with role-based permissions
- **Admin Dashboard** - Complete platform management and analytics
- **Stripe Billing** - Subscription management with per-seat pricing
- **Security Suite** - Bcrypt hashing, Fernet encryption, rate limiting, XSRF protection

---

## Tech Stack

| Component | Technology |
|-----------|------------|
| **Frontend** | Streamlit with custom CSS |
| **Database** | PostgreSQL (Neon-backed) |
| **Authentication** | Custom with bcrypt password hashing |
| **Payments** | Stripe (subscriptions + per-seat billing) |
| **Email** | SendGrid API |
| **SMS** | Twilio API |
| **Calendar** | Google Calendar API |
| **Background Jobs** | APScheduler |
| **Encryption** | Fernet (cryptography) |
| **Analytics** | Plotly, Pandas, NumPy |
| **Hosting** | Replit (with custom domain support) |

---

## Pricing

| Plan | Monthly | Seats | Key Features |
|------|---------|-------|--------------|
| **Starter** | $79 | 1 | Core calculators, basic CRM, deal tracking |
| **Pro** | $149 | 5 | Monte Carlo, drip campaigns, API access, bulk import |
| **Elite** | $249 | 15 | Investor portal, team collaboration, contract templates, priority support |

**Launch Pricing** - Lock in these rates before March 31, 2026.

Additional seats: Pro $12/seat/mo, Elite $15/seat/mo

---

## Quick Start

### Prerequisites
- Python 3.11+
- PostgreSQL database
- Stripe account (for billing)
- SendGrid account (for email)
- Twilio account (for SMS)

### Environment Variables

```bash
# Database
DATABASE_URL=postgresql://user:pass@host:5432/dbname

# Stripe
STRIPE_SECRET_KEY=sk_live_...
STRIPE_PUBLISHABLE_KEY=pk_live_...

# SendGrid
SENDGRID_API_KEY=SG....

# Twilio
TWILIO_ACCOUNT_SID=AC...
TWILIO_AUTH_TOKEN=...
TWILIO_PHONE_NUMBER=+1...

# Security
ENCRYPTION_KEY=your-fernet-key

# Admin
ADMIN_EMAIL=admin@nxtrix.com
```

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/nxtrix.git
cd nxtrix

# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run nxtrix_saas_app.py --server.port 5000 --server.address 0.0.0.0
```

---

## Database Schema

NXTRIX uses a comprehensive PostgreSQL schema with 29 tables:

- `users` - User accounts and authentication
- `contacts` - CRM contacts (leads, buyers, sellers, investors)
- `deals` - Real estate deal records
- `analyses` - Deal analysis calculations
- `tasks` - Task management
- `activities` - Activity logging
- `communications` - Email/SMS history
- `portfolio` - Portfolio holdings
- `investors` - Investor profiles
- `investor_deals` - Investor-deal relationships
- `automations` - Drip campaign configurations
- `billing_history` - Payment records
- And more...

---

## Screenshots

<p align="center">
  <img src="attached_assets/dashboard-preview.png" alt="Dashboard" width="600">
  <br><em>Enterprise Dashboard with real-time KPIs</em>
</p>

<p align="center">
  <img src="attached_assets/deal-analysis-preview.png" alt="Deal Analysis" width="600">
  <br><em>60-second deal analysis with multiple exit strategies</em>
</p>

---

## Why NXTRIX?

| Problem | NXTRIX Solution |
|---------|-----------------|
| Spreadsheet errors cost money | Bulletproof calculations, no formula mistakes |
| Deal analysis takes too long | Analyze in 60 seconds, not 60 minutes |
| No tools for creative finance | Built specifically for Subject-To, Owner Finance, Lease Options |
| Basic "best guess" projections | Monte Carlo runs 1,000+ scenarios |
| Separate CRM and calculators | All-in-one platform |
| Individual tools only | Team collaboration with seat-based pricing |

---

## Comparison

| Feature | BiggerPockets Pro | NXTRIX |
|---------|-------------------|--------|
| BRRRR Calculator | Yes | Yes |
| Fix & Flip Calculator | Yes | Yes |
| Subject-To Analysis | No | **Yes** |
| Owner Finance Calculator | No | **Yes** |
| Monte Carlo Simulation | No | **Yes** |
| Built-in CRM | No | **Yes** |
| Drip Campaigns | No | **Yes** |
| Team Collaboration | No | **Yes** |

---

## Documentation

- [Marketing Plan](MARKETING_PLAN.md) - 90-day organic marketing strategy
- [Marketing Templates](MARKETING_TEMPLATES.md) - Ready-to-use posts and emails
- [Quick Start Marketing](QUICK_START_MARKETING.md) - 7-day launch checklist

---

## Security

- Bcrypt password hashing (12 rounds)
- Fernet encryption for sensitive tokens
- Rate limiting on authentication endpoints
- XSRF protection
- Secure session management
- Input validation and sanitization
- No secrets in code or logs

---

## Support

- **Website:** [nxtrix.com](https://nxtrix.com)
- **Email:** support@nxtrix.com

---

## License

This project is proprietary software. All rights reserved.

Copyright © 2024 NXTRIX. Unauthorized copying, modification, distribution, or use of this software is strictly prohibited.

---

<p align="center">
  <strong>Analyze smarter. Close faster. Scale bigger.</strong>
</p>

<p align="center">
  Built by real estate investors, for real estate investors.
</p>
