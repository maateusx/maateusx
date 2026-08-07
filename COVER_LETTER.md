<div align="center">

# Mateus Pereira

**Senior Fullstack / Applied AI Engineer**

Uberlândia, Brazil · Remote-first · English C1
[mateus1128@gmail.com](mailto:mateus1128@gmail.com) · [LinkedIn](https://www.linkedin.com/in/maateusx/) · [GitHub](https://github.com/maateusx)

</div>

---

Hi,

Most people writing "Applied AI Engineer" on a CV today learned it in the last eighteen months. I've been building conversational systems since 2019 — Dialogflow and Watson first, production LLMs since 2023 — and shipping distributed systems since 2014. That order matters, and it's the whole reason I'm writing to you.

**The thing I'm best at is getting AI systems past the demo.**

At Mobize, the company I founded, I built TakeSales/TakeFlow AI: a multi-tenant platform for voice and chat agents wired into real telephony. A call flows through Twilio → Deepgram streaming STT → an orchestrator doing tool calling and retrieval → ElevenLabs or Gemini Live for speech — and the entire round trip has to land under **900ms**, because past that the human on the phone hears a pause and starts talking over the agent. Hitting that number wasn't a prompt engineering problem. It was turn-taking logic, barge-in detection, speculative synthesis, and ruthlessly cutting retrieval round-trips. The interesting engineering in applied AI is almost never the model call.

The same instinct shows up in retrieval. My RAG is hybrid — semantic plus BM25, reranked with Cohere, tenant-isolated on pgvector — because pure vector search quietly fails on the exact queries users care most about: product codes, proper nouns, contract clauses. And it's instrumented: Langfuse for traces and cost attribution, OpenTelemetry for distributed tracing, RAGAS-based eval suites so a model or prompt change produces a number instead of a vibe. I've also pushed agents into my own CI, where they open and review merge requests.

**Why the systems background is load-bearing.** Before AI, I spent four years as Tech Lead at Bittar Neurociência architecting a full education ecosystem — LMS, CMS, CRM, live and on-demand video — serving thousands of concurrent users on Kubernetes, microservices, event queues, and observability from day one. That's why I reach for a queue, a trace, or a cache boundary by reflex when an AI feature meets real traffic. Plenty of engineers can make an LLM produce a good answer once. Fewer can keep it correct, observable, and affordable at the thousandth concurrent request.

**What I'm actually like to work with.** I write structured specs before I write code — dense enough that the design gets argued with before it gets built, which also makes coding agents genuinely effective rather than chaotic. I own things full-cycle: product shape, architecture, code, infra, deploy, and the pager. Running Mobize means I've also done the parts engineers usually get shielded from — competitive analysis against VAPI and Retell, pitch decks, accelerator applications, choosing a stack for cost and delivery speed instead of taste. I'd rather be told directly that I'm wrong than be agreed with politely.

**What I'm looking for.** A team building AI-first products where the AI is the product, not a feature bolted onto one — and where someone who can hold the whole stack, from the token stream down to the Fargate task definition, is worth more than a specialist in either half. I'm generalist by design and Tech Lead by history, so I'm equally comfortable as a hands-on senior IC or leading a small team.

If you're shipping voice agents, retrieval systems, or agentic infrastructure and you want someone who's already been burned by all three, I'd love to talk.

Best,
**Mateus Pereira**

---

<div align="center">

<a href="https://www.linkedin.com/in/maateusx/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:mateus1128@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="./README.md"><img src="https://img.shields.io/badge/Back_to_profile-0f172a?style=for-the-badge&logo=github&logoColor=white" alt="Profile"/></a>

</div>
