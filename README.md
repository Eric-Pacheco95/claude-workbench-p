# Personal AI Brain -- Starter Kit

A scaffolded AI brain for Claude Code. Skills, learning loops, steering rules, and security -- all working together to make your sessions compound over time.

## What This Is

This is not a chatbot wrapper. It's a **system** that gets smarter the more you use it:

- **35 skills** for research, analysis, building, writing, and learning
- **A learning loop** that captures signals from every session and synthesizes them into steering rules
- **Steering rules** that shape Claude's behavior based on YOUR patterns and preferences
- **Security rules** that protect your data and enforce safe defaults
- **An orchestration layer** for tracking tasks and projects

## Quick Start

```bash
git clone <this-repo>
cd claude-workbench-p
claude
```

Then follow `QUICKSTART.md` for your first 5 sessions.

## Skills by Stage

### OBSERVE (Research & Input)
| Skill | What it does |
|-------|-------------|
| `/research` | Web research with structured output |
| `/absorb` | Ingest articles, videos, posts with dual-lens analysis |
| `/extract-wisdom` | Extract ideas, insights, quotes from any content |
| `/extract-alpha` | Extract the highest-signal, most novel ideas |
| `/analyze-claims` | Fact-check and evaluate claims |

### THINK (Analysis & Planning)
| Skill | What it does |
|-------|-------------|
| `/first-principles` | Deep analytical thinking from fundamentals |
| `/red-team` | Stress-test any plan or proposal |
| `/find-logical-fallacies` | Identify reasoning errors |
| `/architecture-review` | Evaluate architecture decisions |

### PLAN (Design & Specification)
| Skill | What it does |
|-------|-------------|
| `/create-prd` | Collaborative PRD creation with ISC |
| `/project-init` | Full project kickoff pipeline |
| `/delegation` | Route tasks to the right skill |
| `/backlog` | Capture task ideas into the backlog |

### BUILD (Implementation)
| Skill | What it does |
|-------|-------------|
| `/implement-prd` | Build against a PRD's ISC criteria |
| `/review-code` | Code review with security awareness |
| `/quality-gate` | Validate build output against ISC |
| `/commit` | Structured git commits |
| `/self-heal` | Diagnose failures, apply fixes, verify |
| `/security-audit` | Security scan of your codebase |
| `/autoresearch` | Metric-driven improvement loops |
| `/validation` | Run ISC verification commands |

### LEARN (Capture & Synthesize)
| Skill | What it does |
|-------|-------------|
| `/learning-capture` | Capture session signals |
| `/synthesize-signals` | Distill signals into themes |
| `/update-steering-rules` | Turn insights into CLAUDE.md rules |
| `/teach` | Deep-dive lesson on any topic |

### CREATE (Content & Output)
| Skill | What it does |
|-------|-------------|
| `/write-essay` | Long-form writing from any input |
| `/create-keynote` | Presentation deck with speaker notes |
| `/visualize` | Mermaid diagrams from complex inputs |
| `/spawn-agent` | Compose custom agent personas |
| `/create-pattern` | Create new skills |
| `/improve-prompt` | Refine any prompt |

### ORCHESTRATE (Meta)
| Skill | What it does |
|-------|-------------|
| `/help` | Skill registry with search |
| `/project-orchestrator` | Multi-project lifecycle management |
| `/workflow-engine` | Chain skills into pipelines |
| `/deep-audit` | Multi-axis codebase audit |

## Core Pipelines

```
Research:  /research -> /extract-wisdom -> /learning-capture
Build:    /create-prd -> /implement-prd -> /quality-gate -> /learning-capture
Content:  /extract-wisdom -> /synthesize-signals -> /write-essay
Analysis: /first-principles | /red-team | /analyze-claims
```

## The Learning Loop

```
Session work -> /learning-capture -> /synthesize-signals -> /update-steering-rules
                  (signals)            (synthesis)            (better sessions)
```

## Credits & Upstream

This starter kit is inspired by and built on top of [Daniel Miessler's](https://github.com/danielmiessler) open-source work:

- **[PAI (Personal AI Infrastructure)](https://github.com/danielmiessler/PAI)** — Ideal State Criteria (ISC), the "Scaffolding > Model" founding principle, and the personal-AI-brain pattern this kit starts from
- **[The Algorithm](https://github.com/danielmiessler/TheAlgorithm)** — the 7-phase `OBSERVE → THINK → PLAN → BUILD → EXECUTE → VERIFY → LEARN` doctrine
- **[Fabric](https://github.com/danielmiessler/fabric)** — pattern names including `extract-wisdom`, `extract-alpha`, `analyze-claims`, `find-logical-fallacies`, `first-principles`, `improve-prompt`, and `create-pattern`

These projects are public and meant to be built on; this credit points back so others can find and contribute to the upstream work.

## License

MIT
