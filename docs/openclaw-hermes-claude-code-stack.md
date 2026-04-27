# OpenClaw + Hermes + Claude Code

A practical blueprint for turning OpenClaw into a unified agent control plane that can orchestrate:

- **OpenClaw** as the control plane and multi-channel runtime
- **Hermes** as an ACP / agent runtime target
- **Claude Code** as a coding engine for real repository work

This document is intentionally product-oriented. The goal is not just to "support more tools" but to define a cleaner flagship positioning for this fork.

---

## One-line positioning

**OpenClaw as the control plane. Hermes as the runtime path. Claude Code as the coding engine.**

Or more simply:

**A unified agent workstation for chat, orchestration, and code execution.**

---

## Why this stack makes sense

### OpenClaw
Best at:
- gateway / control plane
- multi-channel messaging surfaces
- long-running assistant presence
- session and tool orchestration
- workspace / skills model

### Hermes
Best at:
- ACP-style harness compatibility
- runtime-oriented agent execution flows
- parity pressure from open-source agent communities

### Claude Code
Best at:
- real coding sessions in terminal
- codebase navigation and edits
- debugging and implementation loops
- high-value software tasks people already want to automate

Together, they form a stronger public story than "OpenClaw alone":

1. **OpenClaw owns the assistant surface**
2. **Hermes expands runtime options**
3. **Claude Code gives the stack a strong coding use case**

---

## Recommended product model

### Layer 1 — Control plane
Use **OpenClaw** as the top-level system:
- channel connections
- routing
- permissions / safety policy
- session visibility
- human approval paths
- automation hooks

### Layer 2 — Runtime adapters
Treat **Hermes** and other ACP-capable runtimes as pluggable execution backends.

Suggested mental model:
- OpenClaw decides **where work should go**
- Hermes executes **runtime-oriented agent tasks**
- Claude Code executes **coding-oriented tasks**

### Layer 3 — Specialist engines
Use **Claude Code** for:
- feature implementation
- bug fixing
- refactors
- repo analysis
- PR-ready code work

---

## Best flagship use case

The strongest public-facing story is not general assistant chat.
It is:

## "Launch coding work from chat, route it intelligently, and keep control in one place."

Example flow:
1. A task arrives through Telegram / Discord / Slack / WebChat
2. OpenClaw classifies the work
3. If it is a coding task, OpenClaw routes it to Claude Code
4. If it needs ACP-compatible runtime work, OpenClaw can route it to Hermes
5. Results come back into the same conversation or review flow

This is a much easier story to explain, demo, and promote.

---

## Product naming ideas

### Conservative
- OpenClaw Agent Stack
- OpenClaw Unified Runtime
- OpenClaw Code & Agent Stack

### Stronger / more brandable
- OpenClaw Trinity
- OpenClaw Forge
- OpenClaw Control Plane
- OpenClaw CodeOps Stack

### Recommended direction
**OpenClaw Trinity**

Subtitle:
**OpenClaw + Hermes + Claude Code in one operator workflow**

---

## Suggested architecture

```text
User / Team Chat Surface
    ↓
OpenClaw Gateway / Session Router
    ├─ General assistant flows
    ├─ Hermes runtime path (ACP / harness work)
    └─ Claude Code path (repo / coding work)
            ↓
      review / approve / merge / report back
```

---

## What to build first

### Phase 1 — Product narrative
- define a clean integrated name
- create one architecture page
- create one setup guide
- create one demo path focused on coding-from-chat

### Phase 2 — Routing rules
- detect coding tasks vs general tasks
- route repo work to Claude Code
- route ACP harness work to Hermes
- keep OpenClaw as the approval and reporting layer

### Phase 3 — Safety + workflow polish
- sandbox coding work
- optional worktree / branch isolation
- plan → review → execute flow
- structured result summaries back into chat

### Phase 4 — Promotion
- terminal demo
- before / after workflow graphics
- one-click setup docs
- social launch focused on the coding use case

---

## Recommended repository strategy

### In this repo (`openclaw`)
Use this fork to document the integrated direction and act as the technical backbone.

### In `openclaw-workspace`
Create the productized layer:
- skills
- adapters
- operator workflows
- promotion assets
- launch docs

This split keeps the upstream-heavy codebase and the public-facing product narrative from fighting each other.

---

## Demo idea

A strong demo should show one task only:

> "Fix this failing test suite and open a reviewable change plan."

Demo flow:
1. User sends the request in chat
2. OpenClaw receives and classifies the task
3. Claude Code is selected as the execution engine
4. Hermes remains available as a runtime path for other agent work
5. OpenClaw returns a summary, status, and next action

That demo is much stronger than a broad platform tour.

---

## Recommended tagline options

- **One control plane for chat, agents, and code work.**
- **OpenClaw for orchestration. Hermes for runtime. Claude Code for execution.**
- **Route smarter. Code faster. Stay in control.**
- **From chat to code delivery in one operator workflow.**

---

## Bottom line

If this fork wants a stronger identity, the best direction is:

**Do not position it as just another personal AI assistant fork.**

Position it as:

**an integrated operator stack where OpenClaw coordinates, Hermes extends runtime capability, and Claude Code handles high-value coding execution.**
