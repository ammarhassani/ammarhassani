# Ammar Al-Zahrani

**AML technology & automation specialist.** I'm a software engineer who works inside a bank's compliance function. I find the manual steps in anti-money-laundering work and replace them with tools, pipelines, and models.

Riyadh, Saudi Arabia

---

### What I work on

**Al-Rajhi Bank, Compliance: AML Risk & Control Specialist** · Oct 2025 to present

- I'm the technical resource the AML units go to (investigation, monitoring, reporting). I look for manual bottlenecks and automate them.
- I lead AML strategy where compliance meets technology: transaction monitoring, system modernization, and MIS delivery.
- I bring AI and ML into AML work, including case analysis, scenario threshold tuning, parameter optimization, and false-positive reduction.
- I'm building a way to move paper KYC records into electronic customer due diligence access.
- I produce SAMA ad-hoc regulatory reports that turn complex transaction data into audit-ready output.
- I build BI dashboards, automated reports, and data models where off-the-shelf tools fall short.

**Al-Rajhi Bank, Retail Credit Risk: Quality Assurance Officer** · Sep 2024 to Oct 2025

- Analyzed mortgage and auto-finance application data for trends, anomalies, and risk indicators.
- Validated applications with rule-based checks and transformation pipelines that fed the fraud department.
- Automated reporting with Python, Power Query, and Excel, and built dashboards for credit risk decisions.

---

### AML engineering

#### AML Transaction Reporting · private repository, built for the AML Risk & Control unit

A portfolio of read-only tools that sit on top of the bank's core-banking ledger in the enterprise data warehouse. They aggregate and surface activity for analysts. Detection scenarios and alerting stay in the bank's transaction monitoring platform.

- **Customer activity lookup** (live, reconciled against source): search by customer ID or account for ledger activity, accounts, and blocks. Ships as a Python desktop app, with a parallel Power BI query.
- **Account transfers:** find transfers seven ways, split into internal, local, and international, with direction and purpose, grouped by counterparty.
- **Top spenders:** highest point-of-sale spend over a date range and where it went. Packaged as a Windows executable.
- **Pattern Hub:** sweeps a date range for individuals matching specific typologies and ranks candidates for analyst review. Each rank shows the evidence behind it, and it never files, alerts, or writes back.
- **MIS Workbench:** management information as a picker over a measure and dimension catalog, with generated SQL, query plans, and charts.
- **Warehouse Truth:** a dated, cited record of what the source tables actually contain. Every figure the other tools rely on is measured once and cited from there.

**How it's built:** about 25k lines of Python and 50+ SQL files. Every new query is checked with `EXPLAIN` before it runs, to stay inside the warehouse's workload rules. Totals are reconciled against a direct `SUM` on the ledger before anything is called verified. A single `check.py` runs module self-tests, rejects SQL that names undeclared tables, and catches broken links.

---

### Selected projects

#### [Silni (صِلْني)](https://github.com/ammarhassani/silni_app) · flagship, solo founder-engineer

An Arabic-first Islamic app for keeping family ties (صلة الرحم). **Live on the [App Store](https://apps.apple.com/sa/app/%D8%B5%D9%84%D9%86%D9%8A/id6756042988).**

- **Product:** relatives and interaction tracking, an interactive family tree, scheduled smart reminders, daily streaks, and a free tier plus a MAX subscription.
- **Anees (أنيس):** an AI companion with a written Arabic persona. It shows up at set points in the app (home greeting, after a logged visit or call, after a broken streak) and has counseling modes and a message writer.
- **Admin-driven AI:** Anees's identity, personality sections, model parameters, touch-point prompts, and scenarios live in Supabase tables. I edit them from **silni-admin**, a Next.js dashboard on Vercel, so persona changes ship without an app release.
- **Engineering:** Flutter + Riverpod on the client. Supabase (Postgres, RLS, 180+ migrations) and Deno edge functions for scheduled reminders, smart nudges, push, and a DeepSeek proxy. Firebase Cloud Messaging, RevenueCat, and Sentry.
- Rewritten from an earlier React Native / Expo prototype to Flutter.

#### [Rizq (رِزق)](https://github.com/ammarhassani/Rizq) · in development

A resource-planning suite for Saudi freelancers: proposal studio, client book, income ledger, bilingual invoicing, rate calculator, and a HADAF eligibility tracker.
Next.js 16 · TypeScript · Supabase with RLS on every table · DeepSeek via the Vercel AI SDK · Vitest + Playwright. Arabic-first with full RTL.

#### [Mizan (ميزان)](https://github.com/ammarhassani/Mizan-App)

An iOS daily planner built around prayer times. It has a drag-and-drop timeline with prayer blocks, 8 calculation methods, adhan notifications, and works offline.
SwiftUI · SwiftData · Combine · CoreLocation.

#### [NoiseAnalyzer](https://github.com/ammarhassani/NoiseAnalyzer-TVTC-Version)

A real-time sound analyzer that started as a college project and grew out of my interest in sound engineering. It uses Web Audio FFT to measure dB levels, classify the environment, and flag bass-, treble-, or speech-heavy profiles. Bilingual EN/AR, packaged for Android with Cordova.

#### [Headless Docs CMS](https://github.com/ammarhassani/360KPI-DOCS-CMS)

A block-based documentation CMS in plain JavaScript with no build step. It has heading, paragraph, code, table, and alert blocks, imports a folder of existing docs, and exports the whole project as a ZIP.

---

### Toolkit

**Data & compliance work:** Python · SQL · SAS · Power Query · VBA · Advanced Excel · ETL · data scraping · machine learning · BI / MIS · Power BI · data visualization

**Product engineering:** Flutter / Dart · Supabase (Postgres) · Firebase · TypeScript / JavaScript · React / Next.js · SwiftUI

---

### Credentials

- **Certified Compliance Officer (CCO)**, 3rd Edition, The Financial Academy (2026)
- **National Comprehensive AML/CTF Program**, The Financial Academy & Presidency of State Security (2026)
- **B.Sc. Software Engineering**, TVTC Communications & Information College (2025), GPA 4.45/5
- **Associate Diploma in Computer Science**, King Saud University (2022), GPA 4.26/5. Graduation project (A+): an NFC smart door-tag system with scan-only secured pages.

---

[LinkedIn](https://www.linkedin.com/in/engammaralhassani) · [eng.alhassani@outlook.com](mailto:eng.alhassani@outlook.com)
