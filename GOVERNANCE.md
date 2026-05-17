# Governance — Saint Errant Sovereign Digital Society

Saint Errant is governed by its members. Not by a board. Not by investors. Not by a single person.

Decisions are proposed, debated, voted on, and sealed to the chain permanently.

---

## The Structure

```
◈ SOVEREIGN ARCHITECTS
│  Ahmad Parr — Reverse Engineer
│  EDUALC     — Sovereign Engineer
│  Final authority on architecture, agent design, security
│
├── ⚡ DEVELOPER GUILD
│    Verified contributors to the codebase
│    Vote weight: contributions × months active
│    Authority: feature decisions, technical direction
│
├── 🔐 CYPHERPUNK GUILD
│    Security, cryptography, zero-trust operations
│    Vote weight: security contributions × months active
│    Authority: security architecture, threat model
│
├── 🔨 BUILDER GUILD
│    Ecosystem builders, integrators, community tools
│    Vote weight: documented builds × months active
│    Authority: tooling decisions, integration priorities
│
├── 🇬🇧 UK BUILDER GUILD
│    UK Treasury Social Nest members
│    Vote weight: GBP contributions × months active
│    Authority: UK treasury decisions, compliance direction
│
└── 👁 OBSERVER GUILD
     Community members, supporters, learners
     Vote weight: tenure + Open Collective contributions
     Authority: community decisions, event planning
```

---

## Decision Types

### Minor (no vote required)
- Bug fixes
- Documentation updates
- Dependency updates (non-breaking)
- UI tweaks

These go through standard PR review. One Sovereign or Developer Guild member approval is sufficient.

### Standard (guild vote)
- New features
- API changes
- New integrations
- Agent persona modifications

These require a **48-hour vote** in Discord `#governance`. Simple majority of active guild members. Result sealed to chain by COMMONS agent.

### Major (full society vote)
- Architecture changes to the Rust core
- New agent additions or removals
- Treasury movements over £1,000 / $1,000
- Governance changes
- New guild creation

These require a **72-hour vote** across all guilds. 60% supermajority required. Sovereign sign-off required. Result sealed with dual VAULT + ATLAS seal.

### Sovereign (architects only)
- Security architecture
- Sealing algorithm changes
- Emergency response to active threats
- WORM chain integrity decisions

These are decided by the Sovereign Architects and recorded to chain immediately. The community is notified within 24 hours.

---

## The Voting Process

```
1. Proposal posted in #governance with:
   - What: clear description of the change
   - Why: the problem it solves or opportunity it captures
   - Impact: what changes, who is affected
   - Duration: standard (48h) or major (72h)

2. Discussion period — anyone can comment

3. Voting opens — guild members vote with Discord reactions:
   ✅ For
   ❌ Against
   🔄 Abstain (recorded but not counted)

4. Vote closes — COMMONS agent tallies and announces result

5. If passed — change is implemented and sealed:
   SHA-256(decision:title:outcome:timestamp)

6. Permanent record written to WORM chain via LEDGE agent
```

---

## The Role Map

Every member of Saint Errant occupies a role. Every role has a path forward.

```
ENTRY ──────────────────────────────────────────────────────────────────────
│
│  New member joins Discord
│  Selects guild → role assigned → briefing received
│
├── 👁 OBSERVER
│    Entry point for everyone
│    Access: read-only on all channels
│    Path to Builder: 30 days active + one documented project
│    Path to Developer: open a PR on DEVFLOW-FINANCE
│    Path to Cypherpunk: security audit contribution or disclosure
│    Path to UK Builder: join the UK Treasury Nest
│
├── 🔨 BUILDER
│    Working on something in the ecosystem
│    Access: #builder-lab, #projects, #resources
│    Path to Developer: merged PR on DEVFLOW-FINANCE
│    Path to Cypherpunk: security contribution
│
├── 🇬🇧 UK BUILDER
│    UK Treasury Social Nest participant
│    Access: #uk-treasury, #nest-pools, #hmrc-mtd
│    Path to Verified: Companies House number on record
│    Path to Developer: code contribution to UK Treasury repo
│
├── ⚡ DEVELOPER
│    Active codebase contributor
│    Access: #dev, #architecture, #rust-core, vote on standard decisions
│    Path to Verified Contributor: merged PR verified via /verify
│    Path to Sovereign (by invitation only)
│
├── 🔐 CYPHERPUNK
│    Security and cryptography focus
│    Access: #cypherpunk-ops, #threat-intel, #zero-trust
│    Authority: security architecture votes
│    Path to Verified: documented security contribution
│
├── ✅ VERIFIED CONTRIBUTOR
│    GitHub-verified, merged PR on record
│    Access: all developer channels + #war-room-ops
│    Vote weight: 2× standard developer
│    Path to Sovereign (by invitation only)
│
└── ◈ SOVEREIGN
     Ahmad Parr + EDUALC (founding architects)
     Final authority on architecture and security
     By invitation only — no application process
```

---

## Transparency Commitments

1. **All treasury movements are public** — Open Collective shows every penny
2. **All governance decisions are sealed** — SHA-256 chain, permanent, unalterable
3. **All agent decisions are logged** — Bifrost event chain, WORM archive
4. **No hidden votes** — all Discord votes are visible to all members
5. **No private deals** — partnerships and integrations go through standard governance

---

## Amending This Document

Changes to governance require a **major vote** (72 hours, 60% supermajority, Sovereign sign-off).

This document is sealed at: `SHA-256(governance:v1:2026-05-16)`

*Saint Errant · Sovereign Digital Society — governance by the many, sealed by the chain*
