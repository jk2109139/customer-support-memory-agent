# 🧠 ApexSupport — AI Customer Support Memory Agent

> **Vectorize.io Hindsight Hackathon Project (Option C — Customer Support Memory Agent)**  
> **Live Demo:** [https://customer-support-memory-agent.vercel.app/](https://customer-support-memory-agent.vercel.app/)

ApexSupport is a full-stack AI customer support platform built with **Next.js 14, React, Tailwind CSS**, and the **Vectorize.io Hindsight Memory architecture (Retain, Recall, Reflect)**. 

It solves the single biggest frustration in customer service: **forcing customers to repeat themselves across tickets, device migrations, and multiple support interactions.**

---

## 🌟 Key Features & Hackathon Highlights

1. **"Without Memory" (Stateless) vs. "With Hindsight" Live Toggle:**
   - Instantly switch modes in the top navigation to contrast how standard stateless bots fail vs. how Hindsight retains and recalls past tickets.
2. **Interactive Storyboard (The Rahul Journey):**
   - **Scene 1 (Day 1):** First touch troubleshooting without history.
   - **Scene 2 (Day 15 — The 'Aha!' Moment):** Returning customer with payment issues; Hindsight recalls Ticket #1021 and previous resolution.
   - **Scene 3 (Day 30):** OTP failure on cellular network; Hindsight remembers preference for WhatsApp OTP.
   - **Scene 4 (Day 60):** Customer upgrades device to iPhone 15 Pro; agent links new device to past billing & WhatsApp mandate.
3. **Real-World Live Login (`+ Live Login`):**
   - Enter your own real name, auto-detect your active device/browser, and create a live Hindsight memory bank in real time.
   - AI naturally chats with you, retains your issues into memory, and recalls them when you return!
4. **Hindsight Inspector Drawer:**
   - Real-time diagnostic viewer showing 4-strategy retrieval breakdown:
     - 🎯 **Semantic Similarity** (Cosine distance)
     - 🔍 **BM25 Sparse Retrieval** (Keyword matching)
     - 🕸️ **Causal Knowledge Graph** (Entity & recurrence traversal)
     - ⏳ **Temporal Scoring** (Recency & decay weighting)
5. **Memory Timeline & Customer Profile Sidebar:**
   - Complete visual audit trail of retained entities, customer tier, device environment, and resolution status.
6. **Side-by-Side Comparison Diff:**
   - Live modal demonstrating prompt differences, latency, and response quality between Stateless and Hindsight-augmented agents.

---

## 🏗️ Architecture & How It Works

ApexSupport implements the official **Vectorize Hindsight Triad**:
```
User Query ──► [ Recall ] ──► [ Reflect ] ──► [ AI Agent / LLM ] ──► Response
                  ▲                                    │
                  │                                    ▼
                  └──────────── Memory Bank ◄──── [ Retain ]
```

1. **Retain:** Stores unstructured conversation turns and ticket summaries as structured memory nodes with metadata (ticket ID, resolution, device, sentiment, timestamp).
2. **Recall:** Executes multi-strategy hybrid retrieval (Semantic + BM25 + Graph + Temporal) to fetch top pertinent past solutions.
3. **Reflect:** Synthesizes agent beliefs, customer disposition, and recommended actions before formulating the reply.

---

## 💻 Tech Stack

- **Framework:** Next.js 14 (App Router)
- **Frontend:** React 18, Tailwind CSS, Lucide Icons
- **Memory Engine:** Vectorize Hindsight Client & Embedded High-Fidelity Simulation Engine
- **LLM Layer:** Direct integration with Google Gemini, Groq (Llama 3.1 70B), OpenAI GPT-4o-mini, and built-in Fallback Synthesizer
- **Deployment:** Vercel Global Edge CDN

---

## 🚀 Running Locally

```bash
# 1. Clone repository or unzip files
cd customer-support-memory-agent

# 2. Install dependencies
npm install

# 3. Run development server
npm run dev

# 4. Open in browser
# http://localhost:3000
```

---

## 👥 Hackathon Submission Details

- **Challenge:** Vectorize.io Hindsight Memory Hackathon
- **Track:** Option C (Customer Support Memory Agent)
- **Live URL:** https://customer-support-memory-agent.vercel.app/
