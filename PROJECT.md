# 🚀 TaxCortex - Full-Stack Income Tax Calculator
[![Status](https://img.shields.io/badge/status-production%20ready-brightgreen.svg)](https://taxcortex.com)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

**Full-stack Indian income tax calculator with backend integration, offline capability, and production scalability.** Built for hackathons and deployable in 5 minutes.

## ✨ Features

- **Real-time tax calculations** (FY 2024-25 slabs, old/new regime)
- **6 income sources** (salary, rental, capital gains, freelance, business, other)
- **6×80C investments** (LIC, PPF, NPS, home loan, ELSS, Sukanya Samriddhi)
- **Family tax planning** (multi-member consolidated returns)
- **Quarterly advance tax schedules** (June/Sept/Dec/Mar due dates)
- **Historical YoY comparisons**
- **Offline PWA** with LocalStorage + backend sync
- **PDF/JSON export** for CA filing
- **Docker deployment** (1 command)

## 🏗️ System Architecture (Level 0 DFD)

```mermaid
graph LR
    A[Taxpayer Frontend] -->|JSON Payload| B[Flask Backend APIs]
    B -->|Tax Results| A
    A -->|Offline Backup| C[Browser LocalStorage]
    B -->|Multi-user Data| D[PostgreSQL]
    B -->|Cached Results| E[Redis]

