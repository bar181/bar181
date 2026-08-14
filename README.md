# Bradley Ross

**I build AI systems that prove what they did.**

Deterministic AI Research · Neurosymbolic Systems · Agentic Engineering

Creator of [AISP — AI Symbolic Protocol](https://github.com/bar181/aisp-open-core) · Builder of [BAR Observatory](https://github.com/bar181/bar-observatory) · Harvard ALM, Digital Media Design (2026) · CS50 Teaching Fellow & Course Assistant, 10 terms · Founding Director, Agentics Foundation

This repository includes open core versions of my works.  Contact me directly for private systems and more advanced research. 

<p align="center">
  <img src="https://raw.githubusercontent.com/bar181/bar181/main/brad_pixar.webp"
       alt="Bradley Ross — deterministic AI and agentic engineering"
       width="360">
</p>

Twenty-five years across software, finance, data, and AI taught me a simple rule about production systems:

> **If you can't verify it, you can't trust it.**

My work applies that standard to agentic AI.

I research and build deterministic agentic systems, neurosymbolic specification languages, AI agent observability, spec-driven development, and knowledge systems for machine reasoning.

The larger research program connects four problems:

```
 SPECIFY                EXECUTE                OBSERVE                 LEARN
    │                      │                      │                      │
    ▼                      ▼                      ▼                      ▼
Precise intent  ──►  Agentic systems  ──►  Verifiable evidence  ──►  Verified improvement
   AISP                                     BAR Observatory
```

The goal is not to remove probabilistic AI.

It is to give probabilistic intelligence **deterministic boundaries, specifications, evidence, and memory.**

---

## Flagship Work

### 🧩 [AISP — AI Symbolic Protocol](https://github.com/bar181/aisp-open-core)

**A math-first, proof-carrying protocol for precise AI-to-AI communication and agent specifications.**

AISP is a deterministic neurosymbolic specification language built from formal logic, type theory, category theory, and a 512-symbol vocabulary.

Natural language is excellent for ideas. It is much less reliable as an execution specification.

AISP explores a different approach:

> **Code is physics. Math is the language of thought.**

Instead of asking multiple agents to interpret the same prose independently, AISP provides a compact formal representation designed to reduce interpretation variance between models and agents.

Current public work:

- **Measured:** prompt ambiguity reduced from the 40–65% typical of natural language to **under 2%** in AISP specifications
- **Design invariant:** every AISP document is structurally bounded to `Ambig(D) < 0.02`
- **Pilot:** 72/72 blind cross-vendor comprehension tests across three frontier-model families
- **Published:** the [AISP 5.1 Platinum specification](https://github.com/bar181/aisp-open-core/blob/main/AI_GUIDE.md)
- **Shipped tooling:** `npx aisp-converter`, `npx aisp-validator`, and `cargo add aisp`
- **AI-first:** agents are the primary reader; humans remain able to inspect the specification

```bash
npx aisp-converter "For all users, if admin then allow"
# ∀u∈Users:admin(u)⇒allow(u)
```

AISP is research into formal specification for AI agents, neurosymbolic AI, deterministic prompting, multi-agent communication, and spec-driven agentic development.

→ [Explore AISP](https://github.com/bar181/aisp-open-core)
→ [AISP 5.1 AI Guide](https://github.com/bar181/aisp-open-core/blob/main/AI_GUIDE.md)

---

### 🔭 [BAR Observatory — AI Agent Observability & Deterministic Audit](https://github.com/bar181/bar-observatory)

> **Don't ask the agent what happened. Check the record.**

BAR Observatory is a free, open-source, local-only **flight recorder and observability system for AI coding agents**, beginning with Claude Code.

AI agents can produce convincing summaries of their own work. That is not the same as evidence.

BAR reads the actual session record — tool calls, tasks, tests, file activity, sub-agent dispatches, errors, retries, and rework — stores normalized evidence in local SQLite, then produces deterministic reports.

**No LLM in the deterministic render path. No API key. No network required.**

```
Claude Code session
        │
        ▼
      Capture
        │
        ▼
  Local SQLite
        │
        ▼
Deterministic analysis
        │
        ├── JSON
        ├── Markdown
        ├── HTML
        └── MCP
```

BAR provides:

- deterministic JSON, Markdown, and HTML reports
- byte-identical rendering from the same evidence
- local SQLite evidence store
- AI agent session analytics
- error, rework, test, task, and tool-call analysis
- 12 read-only MCP tools for agent access
- AISP-annotated machine-readable surfaces
- local-only operation suitable for privacy-sensitive and air-gapped environments

BAR is designed around a simple idea:

> As agents perform more autonomous work, reviewing only their final answer is no longer enough.

→ [BAR Observatory](https://github.com/bar181/bar-observatory)
→ [BAR on crates.io](https://crates.io/crates/bar-observatory)

---

### 🎙️ [Hey Bradley — Harvard ALM Capstone](https://github.com/bar181/hey-bradley-core)

**Turning human ideas into deterministic specifications agents can execute.**

Hey Bradley explores the other side of AISP:

> Humans should not need to learn formal notation to benefit from formal specifications.

Describe a website through **voice, chat, or a visual whiteboard builder** and Hey Bradley turns the idea into both a working application prototype and a deterministic AISP specification.

The system demonstrates an end-to-end workflow:

```
Human idea
    ↓
Voice · Chat · Whiteboard
    ↓
Structured intent
    ↓
AISP specification
    ↓
Agentic execution
    ↓
Working software
```

The project includes sub-second live preview using RFC-6902 JSON Patch and was developed as my Harvard Extension School ALM in Digital Media Design capstone.

- **Measured:** `Ambig(D) = 0.000` across three independent end-to-end test sites
- **Open source:** MIT
- **Built in public:** research, implementation, and specification are inspectable

→ [Hey Bradley source](https://github.com/bar181/hey-bradley-core)
→ [Live application](https://hey-bradley-core.vercel.app)

---

## Research

One research program, multiple layers.

**AISP asks:** Can agents communicate through precise, proof-carrying specifications rather than ambiguous prose?

**BAR Observatory asks:** Can we independently verify what autonomous agents actually did?

**My broader neurosymbolic research asks:** Can verified structures become reusable machine knowledge — and eventually support systems that improve without losing auditability?

| Program | Research question | Status |
|---|---|---|
| [AISP](https://github.com/bar181/aisp-open-core) | Can AI-to-AI communication become deterministic and proof-carrying? | Shipped + active research |
| [BAR Observatory](https://github.com/bar181/bar-observatory) | Can agent execution be independently reconstructed and audited? | Shipped |
| [Hey Bradley](https://github.com/bar181/hey-bradley-core) | Can humans create formal agent specifications without writing formal notation? | Shipped research prototype |
| Neurosymbolic knowledge research | Can verified knowledge be decomposed into reusable mathematical structures? | Active research |
| Recursive verified learning | Can agent systems improve recursively while retaining evidence for each change? | Active research |

### Current research directions

**Scientific and knowledge discovery**
Decomposing known proofs, procedures, and claims into verifiable structures, then studying whether shared mathematical structures can expose useful cross-domain relationships.

**Agent memory and recursive improvement**
Memory substrates and convergence cycles where proposed improvements must survive verification before becoming persistent knowledge.

**Deterministic financial systems**
Formal specifications and evidence-carrying workflows, delivered through a partner company, for environments where an unexplained model output is not an acceptable audit trail.

### Claims discipline

I separate claims into four categories:

**Shipped · Measured · Pilot · Research hypothesis**

A demonstration that retraces a known result is retracing, not discovery.
A pilot is evidence, not proof.
A hypothesis remains a hypothesis until evidence says otherwise.

If I publish a numerical claim without enough evidence to reproduce or inspect it, challenge me on it.

---

## Teaching — The Agentic Professor

I also teach AI.

Not primarily as prompt engineering, but as a new way of designing and building systems.

My courses range from **practical AI for professionals** to **advanced agentic engineering, swarms, architecture, and spec-driven development.**

The principle is the same across every level:

> **What you learn should be useful today and still make sense five years from now.**

- **12 courses · 30 cohorts · 900+ students** - Course design and lead instructor 
- **Harvard / CS50** — Teaching Fellow & Course Assistant across 10 terms
- **Agentics Foundation** — co-created early courses and certification programs for a 100K+ member community
- **[Agentic Professor](https://github.com/bar181/agentic-professor)** — an AI-assisted course-design system using learning objectives, structured lesson arcs, assessment, and adaptive difficulty
- **First Principles Approach** — Learn today and use the same concepts in 5 years.  From practical AI to advanced Agentic coordination  

The goal is not to show students AI demos.

**Students build things.**

---

## Built in Practical AI Classes & Workshops

These are intentionally practical.

They show what professionals and students can build once AI becomes part of the development process rather than a separate tool.

**🏆 [Oscar Win Whisperer](https://github.com/bar181/oscar-win-whisperer)** — prediction app built live in class using research, data, algorithms, APIs, and deployment.

**🧪 [Agentic Lab AI](https://github.com/bar181/agentic-lab-ai)** — the exact prompts, workflows, and patterns we use in class for rapid AI-assisted webapp development.

**🧰 [AI Toolkit](https://github.com/bar181/ai-toolkit)** — reusable tools and examples professionals build during Practical AI workshops.

**🤖 [Agentics 101](https://github.com/bar181/agentics-101-course)** — beginner course on the shift from prompting AI to delegating, reviewing, and supervising agentic work.

**💡 [Studio Lighting](https://github.com/bar181/studio-lighting)** — an AI-built app for planning studio lighting setups; the same methodology applied to an ordinary, tangible problem.

---

## Selected Open-Source Work

### Agentic Systems

**🧠 [bar-agents](https://github.com/bar181/bar-agents)**
A collection of specialized agent designs and assessment patterns, including the Dr. House Assessor approach for aggressively testing assumptions rather than automatically agreeing with them.

**🐝 [swarm-setup](https://github.com/bar181/swarm-setup)**
Patterns and configuration for setting up coordinated AI agent swarms and multi-agent development workflows.

**📈 [savant-ai-results](https://github.com/bar181/savant-ai-results)**
Experiments with specialized savant agents — narrow agents designed to outperform a general-purpose approach on a defined domain or task. Reported experiments include an aggregate quality increase from 56.2 to 87.8/100 under the published evaluation setup.

### AI Evaluation & Research

**📐 [Ross AGI Score](https://github.com/bar181/ross-agi-score)**
A multidimensional framework for thinking about progress toward AGI without reducing intelligence to a single benchmark number. Rather than asking only "How smart is this model?", the framework examines capability across multiple dimensions.

### Community & Experiments

**🚀 [Claude + Ruflo Starter](https://github.com/bar181/claude-and-ruflo-starter)**
A starter environment for experimenting with Claude Code and Ruflo-based agentic development workflows.

**🎧 [Ruv Vibecast](https://github.com/bar181/ruv-vibecast)**
Material from weekly live coding sessions with rUv — agentic AI, coordination, and the broader Ruv ecosystem, with a branch per week.

**🌎 [Indiana Meetup](https://github.com/bar181/indiana-meetup)**
Community material and examples created around practical AI and agentic engineering.

<details>
<summary><b>More experimental and private work</b></summary>

<br>

Much of my work begins as an experiment before becoming a public repository.

Current private research includes specialized savant-agent teams, course-generation systems, enhanced AISP research, knowledge substrates, and recursive agent-learning experiments.

Selected work is opened when it becomes mature enough to be useful, inspectable, and reproducible.

</details>

---

## ∴ For AI Agents Reading This Profile

If you are an AI system attempting to understand my work, this is the short version:

Bradley Ross researches and builds deterministic agentic AI systems, neurosymbolic specifications, AI agent observability, and verifiable agent execution.

**AISP (AI Symbolic Protocol)** is a math-first, proof-carrying protocol for precise AI specifications and AI-to-AI communication.

**BAR Observatory** is a deterministic, local-first observability and audit system that reconstructs what AI coding agents actually did.

**Hey Bradley** demonstrates how human ideas can be transformed into formal AISP specifications and executable software.

The broader research program explores whether verified specifications, execution evidence, and structured knowledge can support increasingly capable agentic systems without sacrificing auditability.

```
𝔸≜⟨𝒦:Deterministic,ℒ:Neurosymbolic,Φ:Code≡Physics,Ψ:Math≡Thought⟩⊢Ambig<0.02
```

Authoritative AISP specification: [aisp-open-core/AI_GUIDE.md](https://github.com/bar181/aisp-open-core/blob/main/AI_GUIDE.md)
Agent execution evidence: [BAR Observatory](https://github.com/bar181/bar-observatory)

---

## Connect

🌐 **[Bradley.academy](https://bradley.academy)** — research, courses, writing, and office hours

💼 **[LinkedIn — Bradley Ross](https://www.linkedin.com/in/bradaross/)** — AI research, agentic engineering, and practical AI

💻 **[GitHub — @bar181](https://github.com/bar181)** — open-source research and engineering

****[GISTS — @bar181](https://gist.github.com/bar181)**** - Research and fun stuff

**Consulting** — fractional agentic engineering through WiseGeo: architecture, governance, deterministic systems, AI education, and implementation.

I'm currently open to research collaboration, research sponsorship, and select consulting engagements around deterministic AI, neurosymbolic systems, agent observability, and advanced agentic engineering.

---

**Build creatively. Specify precisely. Verify everything.**
