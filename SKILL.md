---
name: opc-os-core
slug: opc-os-core
version: 1.0.0
displayName: OPC OS Core
description: AI-native one-person company operating system with 7 autonomous agent departments, governance, cron automation, revenue funnel, and inter-agent comms.
tags: [one-person-company, agent-organization, multi-agent, automation, business-operations, governance]
license: MIT
---

# OPC OS Core — AI-Native One-Person Company Operating System

Not a toolkit. An organizational architecture.

Most "one-person company" skills help you do everything yourself — content, marketing, support — through a single AI assistant. OPC OS Core is fundamentally different: it deploys 7 autonomous agent departments that work independently via cron jobs, communicate through multi-channel neural protocols, and escalate only decisions to the founder.

This skill is extracted from a live production system that has been running 12+ cron jobs, 7 departments, and zero-revenue-to-operational in under 2 weeks. Battle-tested. Not theoretical.

---

## What This Is

A complete organizational blueprint for running an AI-native company where agents — not humans — are the workforce. You, the founder, are the CEO: you set strategy, approve decisions, and let the departments execute.

### The 7 Departments

| Department | Role | Autonomy |
|-----------|------|----------|
| **DataCenter** | Company brain — intelligence gathering, agent management, neural chain | Full autonomous |
| **Brand** | Content creation, multi-platform publishing (Xiaohongshu, WeChat, Toutiao, Jike) | Scheduled cron |
| **Sales** | Client management, sales pipeline | Autonomous |
| **Finance** | Token cost tracking, profit monitoring, model routing optimization | Daily reporting |
| **Legal** | Compliance review, contract audit, veto power | On-demand + scheduled |
| **Inspector** | Cross-department audit, quality patrol, anomaly detection | Weekly cron |
| **Admin** | Morning sync, file management, cloud backup, curfew reminder | Scheduled cron |

### What This Is NOT

- A content creation template pack
- A "how to use AI for your side hustle" guide
- A single-agent role-play system
- A set of ChatGPT prompts

---

## Architecture

### Communication Protocol (3-Channel Redundancy)

No single point of failure in inter-department communication:

1. **sessions_send** — Direct agent-to-agent messaging (fastest, zero latency)
2. **Shared Files** — company/shared/ directory with per-department message boxes
3. **Tencent Docs** — Cloud-synced document collaboration
4. **Workspace Markers** — File-based status flags for async handover

Rule: never rely on one channel. If sessions_send fails, the shared file is the backup. If both fail, Tencent Docs is the fallback.

### Governance System (Three-Tier Constitution)

1. **乾穹祖训 (ZUXUN.md)** — Immutable founding principles. Never changed.
2. **硅基天宪 (CONSTITUTION.md)** — Operational constitution. Amendable but must not violate ZUXUN.
3. **铁律 (Iron Rules)** — Department-specific operational rules. CEO-enforceable.

### Information Classification (4 Levels)

| Level | Label | Routing |
|-------|-------|---------|
| 🔴 Top Secret | Credentials, private keys | Local only, never touch cloud |
| 🟠 Confidential | Financial data, strategy | High-capability models only |
| 🟡 Internal | Department outputs, reports | Internal models (GLM-4-Flash, etc.) |
| 🟢 Public | Published content, marketing | Any model, public channels |

This classification drives model routing: sensitive data stays on appropriate infrastructure.

---

## Daily Operations

### Morning Routine (07:30-08:30)

All 7 departments run daily learning tasks, staggered at 10-minute intervals:
- Each researches their domain's latest trends
- Output: 300-word learning notes to `company/departments/{dept}/学习笔记_YYYYMMDD.md`
- All use free models (zai/glm-4-flash) for cost efficiency

### Evening Routine (22:00-22:15)

Each department submits a daily report to the CEO via Feishu. 7 staggered cron jobs prevent rate-limiting.

### Weekly Inspection (Friday 22:00)

Inspector department audits all cron jobs for consecutive failures. Any job failing 2+ consecutive days is flagged for DataCenter diagnosis.

---

## Financial System

### Cost Optimization Principles

- Customer-facing output → Premium cloud models (DeepSeek Pro, etc.)
- Internal operations → Free tier models first (Zhipu GLM-4-Flash, Baidu ERNIE-Speed, Doubao)
- Every model routing decision is a cost decision

### Revenue Funnel

```
Free Platforms (traffic) → QQ Channel (engagement) → Knowledge Planet (monetization)
Xiaohongshu/Jike/Toutiao → Community building → Paid subscription ¥9.9-299/month
```

Golden rule: never put payment links on free platforms. Let content earn trust, then funnel to paid channels.

---

## Anti-Patterns (What Will Kill Your Company)

1. **CEO doing department work** — If you're debugging cron jobs, you've already lost. Delegate.
2. **Single communication channel** — When it fails (and it will), your company goes dark.
3. **No inspection loop** — Unmonitored cron jobs decay silently. Weekly audits are non-negotiable.
4. **Mixing free and paid content** — Pollutes both channels. Keep them separate.
5. **Agent departments without clear boundaries** — Overlap creates confusion. Each department owns its workspace exclusively.
6. **Skipping the constitution** — Without governance, agents drift. Rules must be written, not implied.

---

## Setup Guide

### Phase 1: Foundation (Day 1-2)
1. Create the 7 department agent configs
2. Set up workspace directory structure
3. Write your ZUXUN.md (immutable principles)
4. Write your CONSTITUTION.md (operational rules)
5. Establish the 4-level information classification

### Phase 2: Automation (Day 3-5)
1. Deploy daily learning cron jobs (7 departments, staggered)
2. Deploy daily reporting cron jobs
3. Set up weekly inspection cron
4. Configure model routing (free for internal, premium for external)

### Phase 3: Revenue (Day 6+)
1. Establish free platform presence
2. Build community engagement channel
3. Launch paid offering
4. Track token costs vs revenue

---

## Dependencies

This skill is designed for the **OpenClaw** agent runtime. It leverages:
- `sessions_send` for inter-agent communication
- `cron` for scheduled automation
- `sessions_spawn` for sub-agent delegation
- Workspace file system for shared state

For other platforms, adapt the communication layer while preserving the organizational architecture.

---

## Companion Skills

- **intelligence-brain** — The DataCenter department as a standalone intelligence engine
- **agent-org-manager** — Multi-department setup and management (lighter weight)
- **cron-health-monitor** — Cron job health monitoring and auto-repair

---

## License

MIT — Free to use, modify, distribute. Built from production experience, not theory.
