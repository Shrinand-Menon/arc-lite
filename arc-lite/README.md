# ARC-Lite — Lightweight Automated Risk & Compliance Manager

**ARC-Lite** is a compact, demo-ready Governance, Risk & Compliance (GRC) tool built as a learning-first project. It implements the core operational flows recruiters expect from GRC interns: risk registers, vendor assessments, control mapping, policy lifecycle, incident logs, and audit-ready exports.

> This repository contains the project pitch, sample data, and a demo workflow so you can run a local proof-of-concept quickly.

---

## Why ARC-Lite?
- **Recruiter signal:** shows you understand risk scoring, vendor due diligence, control traceability, and audit artifacts.
- **Learning engine:** teaches practical GRC tasks (scoring, mapping ISO/SOC2 controls, evidence tracking).
- **Product potential:** evolves into a freelance/service offering (SME readiness checks, vendor assessments, ISO prep).

---

## Tech stack (MVP)
- Frontend: **React (Vite)** + Tailwind CSS
- Backend: **Node.js + Express** (or Python FastAPI if you prefer)
- DB: **SQLite** (easy for demos)
- Exports: server-side CSV/PDF (jsPDF or Puppeteer later)
- Dev: Docker optional

---

## Repo structure (planned)
arc-lite/
├─ frontend/
├─ backend/
├─ docs/
│ ├─ screenshots/
├─ examples/
│ └─ sample-data.json
├─ README.md
└─ .gitignore


---

## Quick demo (what this repo includes now)
This initial commit contains:
- Project pitch and structure (this README)
- Example dataset: `examples/sample-data.json` (a prefilled risk register + vendors)
- Placeholders for screenshots in `docs/screenshots/` (replace with your own later)

**How to present the demo:** show the README, then open `examples/sample-data.json` and explain:
1. A few assets with associated risks and scores.
2. A vendor with a computed risk band and suggested controls.
3. A control mapping showing traceability.

---

## How to run (MVP checklist for Phase 1)
1. Clone repo locally.
2. Scaffold backend (Express + SQLite). Implement a `GET /demo/data` endpoint that returns `examples/sample-data.json`.
3. Scaffold frontend (Vite + React). Add a simple dashboard that fetches `/demo/data` and renders the risk register and vendor list.
4. Add a screenshot of the running UI into `docs/screenshots/` and update the README.

(If you want, I will scaffold the backend and frontend files next — see "Next steps" below.)

---

## Examples (what to include in sample-data.json)
- 3 assets (e.g., "Student Answers DB", "Web UI", "Storage Bucket")
- 6 risks across those assets
- 2 vendors (one low/one high)
- 4 controls (Access control, Logging, Backup, Incident response)
> `examples/sample-data.json` already contains a small dataset — open it to preview.

---

## Next steps (do this after you push README)
1. Add actual screenshots to `docs/screenshots/` (2–3 images: dashboard, risk register, vendor score).
2. Create branch `feature/scaffold-backend`.
3. Scaffold minimal backend: implement `GET /demo/data` that returns `examples/sample-data.json`.
4. Create branch `feature/scaffold-frontend` and scaffold a minimal React app that fetches and renders the demo data.

---

## Contacts & attribution
Created by: **Eather** — student building a GRC portfolio project  
Repo goal: deliver a demo-ready project for internships and an eventual product path.

