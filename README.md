# NetGuardian AI: Security Research Assistant

**Live Demo:** [https://cf-ai-agent-researcher.dmitry92vr.workers.dev/](https://cf-ai-agent-researcher.dmitry92vr.workers.dev/)

## Overview
NetGuardian AI is a stateful security assistant built for the Cloudflare 2026 Internship assignment. It is designed to help developers identify "cracks" in their infrastructure and provide guidance on security best practices.

## Key Technical Features
- **Stateful Persistence:** Leveraging **Cloudflare Durable Objects** and a SQL database to maintain conversation context across sessions. (Try asking "What is my name?" after a refresh!)
- **Edge-Native Inference:** Runs on **Llama 3.1-8b** via **Cloudflare Workers AI**, ensuring low-latency responses globally.
- **Security-First Persona:** Custom-prompted to identify vulnerabilities like client-side data tampering and SQL injection.

## Tech Stack
- **Framework:** Cloudflare Agents SDK
- **Runtime:** Cloudflare Workers
- **Database:** Durable Objects (SQL)
- **Frontend:** React + Vite

## Development & Deployment
The project was developed in a local Mac environment using `wrangler` and deployed directly to the Cloudflare Global Edge.

### How to run locally:
1. `npm install`
2. `npm run dev`
3. `npm run deploy` to push changes to production.
