# GramSaathi

**An Agentic AI job-matching assistant for rural youth**

> GAVS Hackathon (HackCulture) | Elimination Round: Idea Submission
> **Theme:** Youth and Women
> **Problem Statement:** 8.2 Rural youth cannot find work that fits, and small employers cannot find them

---

## Overview

Rural youth often can't find work because they don't know which jobs exist, which skills employers want, or how to prove their abilities without a formal resume or good internet.

GramSaathi is a multilingual, voice-first AI agent that works through WhatsApp or a lightweight app and acts as a personal career assistant for each young person. Unlike a static job portal, it uses autonomous AI agents that plan, act and follow up on behalf of the user.

## Problem

Millions of rural youth in India are educated or semi-skilled but remain unemployed or underemployed. The main barriers are:

- No awareness of available jobs, schemes and training
- No formal resume, digital presence or interview experience
- Language barriers, as most job portals are English-first
- Limited internet access and low digital literacy
- Mismatch between local skills and local employer demand
- For young women: safety concerns, mobility limits and a lack of trusted, flexible options

## Solution

GramSaathi works in four steps:

1. **Profiles the user** through a simple conversation in their own language, with no resume needed.
2. **Finds opportunities** by searching government schemes (PMKVY, DDU-GKY, NRLM), local employers, gig platforms and apprenticeships, and matching them to the profile.
3. **Closes skill gaps** by recommending free, short training and tracking progress.
4. **Handles the paperwork** by building a digital profile, applying on the user's behalf, preparing them for interviews with mock voice practice, and following up on applications.

A separate agent for employers and local NGOs posts verified openings and flags unfilled demand, so the system adapts to local job markets.

## Agent Workflow

| Agent | Role |
|---|---|
| **Profiling Agent** | Talks to the user by voice or text in their own language (Hindi, Kannada, Tamil, Telugu, Bengali, etc.) and builds a skill profile from education, experience, interests, location and availability. |
| **Opportunity Agent** | Aggregates government schemes (PMKVY, DDU-GKY, NRLM, NCS portal), apprenticeships, local employers, MSMEs, gig platforms and work-from-home options, ranked by fit, distance and pay. |
| **Skill-Gap Agent** | Compares the profile with job requirements, recommends free local-language courses, tracks progress and re-matches as skills improve. |
| **Application Agent** | Generates a digital profile and resume, fills applications and sends them with the user's consent. Sends deadline and document reminders. |
| **Interview Coach Agent** | Runs mock interviews by voice and gives feedback on communication and confidence. |
| **Employer and NGO Agent** | Lets verified employers, SHGs, NGOs and training centres post openings, and analyses unfilled demand so training matches real jobs. |
| **Safety and Trust Layer** | Verifies employers, flags fraudulent offers, and highlights women-friendly roles (safe workplaces, flexible hours, home-based work). |

## Key Features

- Voice-first and multilingual, usable by low-literacy users
- Works on basic smartphones and low bandwidth via WhatsApp
- Agentic automation: search, match, apply, follow up
- Gender-inclusive design with job safety verification
- Local-demand intelligence that links training with real vacancies
- Human-in-the-loop option through village-level coordinators and Common Service Centres

## Tech Stack

| Layer | Technology |
|---|---|
| Agent orchestration | LangGraph / CrewAI with tool calling |
| Speech and language | Bhashini APIs or Whisper (speech-to-text), TTS for Indian languages |
| Channel | WhatsApp Business API |
| Matching | Embeddings plus a vector database (FAISS / Pinecone) |
| Backend | Python (FastAPI), PostgreSQL |
| Data sources | Public scheme portals, employer submissions, job APIs |
| Privacy | Consent-based data use, encryption of personal data |

## Impact

- Reduces job-search time and cost for rural youth
- Improves quality of job matches and placement rates
- Connects skilling programmes to actual local demand
- Increases women's participation in the workforce
- Scales to many districts at low cost because agents do work that needs coordinators today

## Roadmap

- [ ] **Phase 1:** WhatsApp chatbot with profiling, job matching and scheme discovery in 2 languages
- [ ] **Phase 2:** Skill-gap recommendations, resume generation and mock interview coach
- [ ] **Phase 3:** Employer dashboard, safety verification and a pilot with a few villages or an NGO partner

## Future Scope

- Offline-first mode
- More Indian languages
- DigiLocker integration for verified credentials
- Partnerships with state skill missions and local panchayats

## Getting Started

> The prototype is under development. Setup instructions will be added in Phase 1.

```bash
git clone https://github.com/<your-username>/gramsaathi.git
cd gramsaathi
```

## Team

- Add team member names and roles here

## References

- [Bhashini (Indian language AI)](https://bhashini.gov.in)
- [National Career Service](https://www.ncs.gov.in)
- [Skill India](https://www.skillindia.gov.in)

## License

MIT License. Add a `LICENSE` file to the repository.
