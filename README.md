# Ahmad Sleiman

**Software engineer based in Ghana — backend and AI.** I build the server side of web products: APIs, data models, authentication, and the AI layers on top of them. Python and Django are where I work; I ship the frontend when a project needs it, but the backend is the part I'm hired for.

Right now I'm building **[Lahja](https://lahjja.com)** — an AI-powered platform for learning spoken Arabic dialects.

---

## Lahja — AI Arabic dialect coach

**[lahjja.com](https://lahjja.com)** · live

Most language apps teach Modern Standard Arabic, which nobody speaks at home. Lahja teaches the Arabic people actually use — Egyptian, Levantine, Gulf, Moroccan, Iraqi and Tunisian.

- **AI dialect coach** — conversation practice with instant correction and transliteration
- **Live tutoring** — 1-on-1 sessions with verified native speakers
- **Structured curriculum** — A1 to C2, with grammar notes and cultural context
- **Daily practice** — spaced-repetition flashcards, daily challenges, games
- **Progress tracking** — weekly analysis of weak points and a personalised plan

Built solo. The backend is **Django** — accounts and auth, curriculum delivery, tutor scheduling, progress data, subscription entitlements, and the API. The **AI layer** is the harder half: keeping a language model inside one Arabic dialect for a whole conversation, when general-purpose models drift toward Modern Standard Arabic by default. React frontend on top, deployed behind Cloudflare.

*Source is private — I'm happy to walk through the code or give access on request.*

📄 **[Read the full case study →](https://github.com/ahmadtsleima/lahja-case-study)**

---

## Document Intelligence Agent — RAG over PDFs

Ask questions about a PDF and get answers grounded only in that document — with an honest *"I couldn't find that in the document"* when the answer isn't there. That refusal is the point: a model that leaks its training knowledge instead of admitting a gap is a liability.

- **FastAPI**, async throughout — every call that leaves the process releases the worker
- **PostgreSQL + pgvector** for 3072-dimensional similarity search, no separate vector database
- Chunking with overlap so a sentence on a boundary survives intact
- Retrieval grounds the model; the prompt gives it a legal way to say "I don't know"
- UUID filenames on disk, closing both overwrite collisions and path traversal

**Python · FastAPI · PostgreSQL/pgvector · SQLAlchemy async · Gemini · Docker**

📄 **[Read the full case study →](https://github.com/ahmadtsleima/doc-agent-case-study)**

---

## IMS — FIFA World Cup 2026

**[imsworldcup.com](https://imsworldcup.com/en)** · live

A live World Cup companion — real-time scores, group standings, the knockout bracket, top scorers, stadiums and a news feed, in English and Arabic.

- **Live match data** from API-Football, cached and normalised by a **Django** backend so burst traffic at kickoff doesn't hit the upstream API
- **Push notifications** for match alerts, scheduled server-side against fixture times that move
- **Installable PWA** — service worker and manifest, so it behaves like a native app on a phone
- **Bilingual EN/AR** with full right-to-left layout
- Next.js frontend, server-rendered for fast loads on match pages

**Django · Next.js · PWA · API-Football**

*Freelance work. Source is private — available on request.*

📄 **[Read the full case study →](https://github.com/ahmadtsleima/ims-worldcup-case-study)**

---

## Jaafar Sleiman — photographer portfolio

**[jaafarsleiman.com](https://jaafarsleiman.com)** · live

A commissioned portfolio site for a photographer and filmmaker — an editorial black-and-white studio presence built around motion.

- Interactive **before/after colour-grading** slider — drag through the frame to compare neutral capture against the finished grade
- Vertical reel and filmmaking showcases with cinematic pacing
- Categorised photography archive — food, commercial, jewellery, product
- **Django** backend with an authenticated admin panel so the client uploads, categorises and reorders their own work
- Client-side image compression on upload to keep a media-heavy gallery fast

**Django · React 19 · Vite · Three.js/OGL · Docker**

*Source is private — available on request.*

---

## Tech I work with

**Backend** — Python · Django · FastAPI · REST APIs · authentication & authorisation · JWT · bcrypt · Node.js · Express

**AI** — RAG · vector search & embeddings · LLM integration · prompt design and constraint · conversational systems

**Data** — PostgreSQL · pgvector · SQLAlchemy (async)

**Infrastructure** — Docker · Cloudflare Workers · Railway · Fly.io · Vercel · PWA & push notifications

**Also comfortable in** — React · Next.js · JavaScript · Vite · Three.js / WebGL

**Languages** — Arabic (native) · English

---

## Get in touch

- 🌐 **[lahjja.com](https://lahjja.com)**
- 📧 **ahmadsleiman562@gmail.com**

**Open to software engineering roles — backend and AI.**
