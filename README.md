## Joshua van Straaten

Backend and AI engineer in South Africa (UTC+2). I build complete vertical systems — data
ingestion, backend services, LLM integration and shipped product — and I make engineering
decisions with measurements rather than assumptions.

Currently a Data Engineer at Snode Technologies, building ETL/ELT pipelines and a medallion
lakehouse over security data. Previously three years at Corigine writing RISC-V firmware in C
and owning the team's CI/CD. Alongside that I design, build and operate three production
systems of my own.

**Open to fully remote roles worldwide.** → [joshuavanstraaten.com](https://joshuavanstraaten.com)

---

### What I'm building

**[HanVoice](https://github.com/JoshuaVanStraaten/hanvoice)** — Korean pronunciation-learning
PWA, live at [hanvoice.app](https://hanvoice.app) with paying users.
FastAPI on Fly.io, React PWA on Vercel, PostgreSQL on Supabase. Real-time pronunciation scoring
over Azure Speech, plus two LLM features: a conversational practice partner and a vision-model
pipeline that reads handwritten Hangul from photographs. 126 backend tests, mypy strict, ruff clean.

**Pettlo** *(private — client work)* — Multi-tenant veterinary SaaS with AI-generated clinical
notes. Consultation audio → speech-to-text with diarization → Claude → structured clinical notes,
with explicit gap detection so the model flags missing information rather than inventing it.
Tenant isolation enforced in two layers via PostgreSQL row-level security. 543 tests.

Two results I'm proud of there:
- A five-vendor speech-to-text evaluation that cut **word error rate from 6.2% to 3.1%** and
  per-customer cost by **64%** — and surfaced a silent production defect where mismatched
  language codes were quietly generating notes in the wrong language.
- **A row-level-security optimisation from 727ms to 6.2ms (117×)** on a 50k-row benchmark, by
  hoisting per-row policy function calls into a per-query InitPlan, plus covering indexes for
  twelve unindexed foreign keys.

**[Milk](https://github.com/JoshuaVanStraaten/milk)** — Flutter app on Google Play comparing live
grocery prices across five South African retailers. Riverpod + Supabase, with a
[Python scraping and normalisation layer](https://github.com/JoshuaVanStraaten/retailer-scrapers)
that reconciles inconsistent product naming, packaging and units, and a fallback service layer so
upstream retailer outages degrade gracefully.

---

### Tools

**Languages** Python · TypeScript · Go · C/C++ · SQL · Dart
**Backend** FastAPI · Next.js · PostgreSQL · Supabase · Stripe · REST API design
**AI/LLM** Claude API · Gemini · RAG · model evaluation & benchmarking · speech-to-text · vision models
**Data** ETL/ELT · medallion architecture · Elasticsearch · Vector · data quality validation
**Infra** Docker · GitHub Actions · Ansible · Fly.io · Vercel · Cloudflare · Sentry · PostHog

---

### Elsewhere

[Portfolio](https://joshuavanstraaten.com) · [LinkedIn](https://www.linkedin.com/in/joshua-van-straaten) · joshuavanstraaten100@gmail.com
