# Contributing to Saint Errant

Welcome. You found us. That means something.

Saint Errant is a sovereign digital society — non-profit, open source, community-governed. Everything we build is public. Everything we decide is sealed to a chain. Everyone who contributes leaves a permanent mark.

This guide tells you how to become part of that.

---

## Before You Start

Read the [README](README.md). Understand what we are and what we are not.

We are not a startup. We are not building for a pitch deck. We are not chasing users. We are building sovereign infrastructure for people who understand why sovereignty matters.

If that resonates — you're in the right place.

---

## Ways to Contribute

### Code
The main codebase lives at [DEVFLOW-FINANCE](https://github.com/SNAPKITTYWEST/DEVFLOW-FINANCE).

- **Rust core** — the sealing engine, WORM ledger, tier state machine
- **TypeScript/Next.js** — the War Room, agent system, API layer
- **Discord bot** — the community gateway at [myapplication](https://github.com/SNAPKITTYWEST/myapplication)
- **UK Treasury** — the GBP capital and compliance layer

### Community
- Answer questions in Discord — `discord.gg/dugymT3rj`
- Help new members find their guild
- Write documentation and guides
- Translate content

### Research
- Cryptographic sealing improvements
- Local LLM optimisation (Ollama model selection, quantisation)
- UK financial regulation and compliance research
- Open Banking and PSD2 integration

### Design
- UI/UX for the War Room and community hub
- Branding assets for the guilds
- Documentation diagrams and architecture visuals

### Funding
- Contribute on [Open Collective](https://opencollective.com/snap-kitty-infrastructure-netw)
- Every contribution is public, tracked, and goes directly to infrastructure

---

## Getting Started

### 1. Join Discord
```
discord.gg/dugymT3rj
```
Declare your guild. Get your role. Introduce yourself in `#introductions`.

### 2. Fork the repo

```bash
git clone https://github.com/SNAPKITTYWEST/DEVFLOW-FINANCE.git
cd DEVFLOW-FINANCE/collectivekitty
npm install
npx prisma generate
```

### 3. Create a branch from `main`

```bash
git checkout main
git pull origin main
git checkout -b feat/your-feature-name
```

Never branch from another feature branch.

### 4. Make your change

Keep it focused. One feature, one fix, one improvement per PR. No drive-by refactors.

### 5. Test it

```bash
npm run dev       # start the server
npm run lint      # check for errors
npm test          # run the test suite
```

### 6. Open a pull request

Use the PR template. Fill it out. Be specific about what changed and why.

---

## Code Standards

**TypeScript**
- Strict mode — no `any` without a comment explaining why
- No secrets in code — all credentials via environment variables
- No comments explaining what the code does — only why, when it's non-obvious

**Rust**
- `cargo clippy` must pass before PR
- No `unsafe` without sign-off from a Sovereign
- Deterministic IDs only — no `SystemTime`, no `rand` in the core

**Git**
- Commits in present tense: `feat: add X` not `added X`
- No force-pushing to `main`
- No `--no-verify` skipping hooks

**Security**
- Never commit credentials, tokens, or keys
- Ed25519 verification on all Discord interactions — non-negotiable
- SHA-256 sealing on all agent decisions — non-negotiable

---

## Governance

Major decisions go through COMMONS — our governance agent. Proposals are posted in `#governance` in Discord, voted on by guild members, and the result is sealed to the chain.

Minor contributions (bug fixes, docs, small features) go through standard PR review.

Sovereign-level decisions (architecture changes, agent modifications, treasury movements) require sign-off from the core architects.

See [GOVERNANCE.md](GOVERNANCE.md) for the full process.

---

## First Contribution?

Look for issues tagged `good first issue` or `guild: observer`.

Or just ask in `#dev` in Discord — someone will point you at something real to work on.

---

## Recognition

Every contributor is recorded in the chain. Verified contributors get:
- `@Verified Contributor` role in Discord
- Name in the contributor list
- Permanent record in the WORM ledger

Run `/verify github-username:YourHandle` in Discord after your first merged PR.

---

*Saint Errant · Sovereign Digital Society*
*We build in the open. The chain remembers everyone who contributed.*
