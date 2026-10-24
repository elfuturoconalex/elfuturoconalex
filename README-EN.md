# Hi, I'm Alejandro

**Solutions Architect in Networking & Data Center → Building AI Agents on AWS**

🇲🇽 [Leer en español](README.md)

I'm a technology professional with years of experience as a **pre-sales architect** at a **Cisco partner**, designing **networking** and **data center** solutions. My work sits between two worlds: the technical and the human — understanding what a client needs and turning it into a solution people can understand and decide on.

Now I'm bringing that same approach to AI: building agents that small businesses can actually trust, that run 24/7 on AWS, and that cost cents per conversation.

### What I bring
- **Networking:** Cisco architectures and solution design
- **Data center:** Dell, Lenovo, Everpure Storage
- **Backup & data protection:** Veeam, Commvault
- **Virtualization:** VMware, Red Hat
- **Communication:** explaining complex technology in a way people can act on

### What I'm building
I'm learning to **build AI agents and deploy them on AWS** — starting from zero in programming. My goal: **5 AI agents**, each one more complex than the last. *(Project docs are in Spanish, each with an English summary.)*

| # | Project | Status |
|---|---|---|
| 1 | [**Research Agent**](https://github.com/elfuturoconalex/agente-investigador) — searches the web and writes a report with its sources. Using traces, I cut its cost per report by 22% | ✅ Local · ✅ AWS (Bedrock) |
| 2 | [**Internal Support Agent**](https://github.com/elfuturoconalex/agente-soporte-interno) — answers employee questions from company documents (RAG on Bedrock + Lambda + API Gateway). Cites the source document and says "I don't know" instead of inventing | ✅ Done · **25/25** on automated eval |
| 3 | [**Telegram Ordering Agent**](https://github.com/elfuturoconalex/agente-pedidos-telegram) — takes orders the way customers actually talk, checks a real catalog, confirms address and payment, and saves each order with a folio number | 🔄 Phase 1 of 3 · **8/8** on automated eval |
| 4–5 | Coming soon | ⏳ |

*All demos use fictional companies and data.*

### What building them taught me
- **AI doesn't fail for lack of intelligence — it fails for lack of data and controls.** Money and business rules are decided by code, not by the model.
- **A rule in the prompt isn't enough.** My ordering agent said "your order is confirmed" before saving anything. A guard in code fixed it.
- **AI remembers what it said, not what it did.** It forgot it had already added an item and added it again. Now the code keeps the order state and shows it to the model on every message.
- **No eval, no trust.** A conversation that looked perfect was saving orders at double the price. Only automated tests caught it.
- **A well-built agent costs cents per conversation.**

**Stack:** Python · Claude API · Amazon Bedrock · RAG · AWS Lambda · API Gateway · S3 · CloudWatch · Tavily · Telegram Bot API · Git/GitHub · Terraform (in progress)

### Where I'm going
Building a "T-shaped" profile: broad foundations in cloud, networking, data center, security and cost — with deep expertise in **AI agents on AWS**. Long term: **Solutions Architect specialized in AI**, helping small businesses in Mexico and Latin America put agents to work.

### Let's talk
Want to bring AI agents to your business, or need an AI architect on AWS?
👉 [LinkedIn](https://www.linkedin.com/in/yosoyalexpadilla/) · I share the journey in Spanish as **El Futuro con Alex**

📖 [Read my full story](MY-STORY.md)

> At 45, I'm not starting from scratch — I'm adding a new layer to everything I've already built.
