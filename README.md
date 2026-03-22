# Template: Executive Agent

> Enable strategic decisions with portfolio oversight and resource allocation

**Version**: v3.10.0 | **Archetype**: Executive | **Skills**: 2 specialized + 15 universal

---

## Why Executive?

The Executive archetype provides **strategic decision support** at the organizational level. Unlike tactical advisors, executive agents handle:

- **Decision authority** — Structure decisions with clear options, criteria, and accountability
- **Budget oversight** — Review resource allocation against strategic priorities
- **Portfolio thinking** — Balance competing initiatives across the organization

**For evaluators**: If you need an AI that can support high-level strategic decisions with appropriate rigor and documentation, the Executive archetype provides leadership-grade decision support.

**Domain knowledge that compounds**: Executive agents build persistent understanding of your strategic landscape — past decisions, resource allocation outcomes, and portfolio priorities. Unlike tools that start fresh each session, your agent accumulates strategic context that makes each decision better framed and each budget review more informed.

---

## Skills

Executive agents come with **2 archetype-specific skills** plus the universal AGET skills.

### Archetype Skills

| Skill | Description |
|-------|-------------|
| **aget-make-decision** | Structure decisions with options, criteria, and documented rationale. Supports go/no-go decisions with accountability. |
| **aget-review-budget** | Review budget allocation against strategic priorities. Identifies gaps, overruns, and reallocation opportunities. |

### Universal Skills

All AGET agents include session management, knowledge capture, and health monitoring:

- `aget-wake-up` / `aget-wind-down` — Session lifecycle
- `aget-create-project` / `aget-review-project` — Project management
- `aget-record-lesson` / `aget-record-observation` — Learning capture
- `aget-check-health` / `aget-check-kb` / `aget-check-evolution` — Health monitoring
- `aget-propose-skill` / `aget-create-skill` — Skill development
- `aget-save-state` / `aget-file-issue` — State and issue management

---

## Ontology

Executive agents use a **formal vocabulary** of 6 concepts organized into 2 clusters:

| Cluster | Concepts |
|---------|----------|
| **Strategic Decision** | Decision, Criteria, Outcome |
| **Resource Management** | Budget, Portfolio, Priority |

This vocabulary enables precise communication about strategic choices.

See: [`ontology/ONTOLOGY_executive.yaml`](ontology/ONTOLOGY_executive.yaml)

---

## Quick Start

```bash
# 1. Clone the template
git clone https://github.com/aget-framework/template-executive-aget.git my-executive-agent
cd my-executive-agent

# 2. Configure identity
# Edit .aget/version.json:
#   "agent_name": "my-executive-agent"
#   "domain": "your-domain"

# 3. Verify setup
python3 -m pytest tests/ -v
# Expected: All tests passing
```

### Try the Skills

```bash
# In Claude Code CLI
/aget-make-decision    # Structure a strategic decision
/aget-review-budget    # Review resource allocation
```

---

## What Makes Executive Different

| Aspect | Tactical Advisor | Executive Agent |
|--------|-----------------|-----------------|
| **Scope** | Single issues | Portfolio-wide |
| **Decisions** | Recommendations | Structured decision frameworks |
| **Resources** | Not considered | Budget/allocation focus |
| **Accountability** | Advisory only | Decision documentation |
| **Domain memory** | Starts fresh each session | Accumulates strategic expertise over time |

---

## .claude/ Directory

| Directory | Purpose | Owner |
|-----------|---------|-------|
| `.claude/skills/` | Slash command definitions | Framework + Agent |
| `.claude/agents/` | Subagent definitions | Agent |
| `.claude/rules/` | Path-scoped context rules | Agent |

Skills are provided by the template. Agents and rules directories are scaffolded for your customization.

---

## Framework Specification

| Attribute | Value |
|-----------|-------|
| **Framework** | [AGET v3.10.0](https://github.com/aget-framework/aget) |
| **Archetype** | Executive |
| **Skills** | 17 total (2 archetype + 15 universal) |
| **Ontology** | 6 concepts, 2 clusters |
| **License** | Apache 2.0 |

---

## Learn More

- **[AGET Framework](https://github.com/aget-framework/aget)** — Core framework documentation
- **[Archetype Guide](https://github.com/aget-framework/aget/blob/main/docs/GETTING_STARTED.md)** — All 12 archetypes explained
- **[Getting Started](https://github.com/aget-framework/aget/blob/main/docs/GETTING_STARTED.md)** — Full onboarding guide

---

## Related Archetypes

| Archetype | Best For |
|-----------|----------|
| **[Supervisor](https://github.com/aget-framework/template-supervisor-aget)** | Fleet coordination and oversight |
| **[Advisor](https://github.com/aget-framework/template-advisor-aget)** | Risk and recommendation support |
| **[Consultant](https://github.com/aget-framework/template-consultant-aget)** | Engagement and proposal creation |

---

**AGET Framework** | Apache 2.0 | [Issues](https://github.com/aget-framework/template-executive-aget/issues)
