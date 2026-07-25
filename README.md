# Dakota Smith

### I build things that build things.

Agentic systems for organizations that can't afford to get it wrong.

---

## The problem I keep working on

Every organization wants agents doing real work. Almost none of them can answer the question that follows: how do you let an agent act without losing the ability to say what happened, why it was allowed, and whether it was correct.

That answer is infrastructure, not prompting. Permission before the act, evidence after it — recorded on one log, replayable rather than asserted. Agents propose, humans dispose, and everything an agent touches leaves a trail you can audit later.

```mermaid
flowchart LR
    A["Agent proposes"] --> P{"Permit"}
    P -->|allow| X["Act"]
    P -->|deny| S["Blocked"]
    X --> E["Evidence"]
    E --> H["Human disposes"]
    H --> L[("One auditable log")]
    S --> L

    classDef permit fill:#3B82F6,stroke:#1D4ED8,color:#fff
    classDef good fill:#10B981,stroke:#047857,color:#fff
    classDef stop fill:#EF4444,stroke:#B91C1C,color:#fff
    classDef log fill:#6366F1,stroke:#4338CA,color:#fff
    class P permit
    class E,H good
    class S stop
    class L log
```

I've built it four different ways, in two languages, to find out which parts hold up.

## Selected work

| Project | What it is | Status |
|---|---|---|
| **[rezidnt](https://github.com/rezidnt/rezidnt)** | A local-first daemon running a fleet of coding agents under policy — permission checked before every action, evidence recorded after, both on one auditable log. Rust. | ![alpha](https://img.shields.io/badge/alpha-F59E0B?style=flat-square) |
| **[Dossier](https://github.com/smithdak/dossier)** | Institutional memory an organization owns outright — agents extend it, humans approve, and approved work compounds into the company's own git history. | ![beta](https://img.shields.io/badge/beta-3B82F6?style=flat-square) |
| **[ObjectCore](https://github.com/smithdak/objectcore)** | A software factory for AI tooling whose output isn't plugins — it's the system that produces and governs them. Live registry, 14 plugins. | ![live](https://img.shields.io/badge/live-10B981?style=flat-square) |
| **[Skillsmith](https://github.com/smithdak/skillsmith)** | A compiler and quality gate for agent skills — schema, security, and trigger evals all run before anything ships. | ![live](https://img.shields.io/badge/live-10B981?style=flat-square) |

## Writing

[daksmith.dev](https://daksmith.dev/) — orchestration patterns, agent tooling, harness design, and the security model underneath it. Most recently on durable agent orchestration: moving coordination into workflow steps instead of trusting a coordinator agent to hold it together.

## Before this

Shipping enterprise digital platforms since 2012 — Sitecore, Umbraco, Optimizely, .NET, Azure — for organizations where the constraints were real and the rollback plan mattered.

That part is what most AI work is missing.

---

[daksmith.dev](https://daksmith.dev/) · [LinkedIn](https://www.linkedin.com/in/dakota-smith-a855b230)
