# Release Notes Skill

A Claude skill that turns raw engineering notes into **clean, audience-correct release notes and launch comms** — classified (New / Improved / Fixed / Deprecated), written separately for the audiences that diverge (admin, end user, developer), in a plain-verbs no-hype voice matched to your product's terminology. Anything the source notes don't establish goes back to engineering as a question — never forward to customers as a guess.

Distilled from owning technical writing for a product's most technical surfaces — endpoint agent, admin console, automation engine, and public API — where release notes shipped ahead of schedule.

## What it does

- **Classifies** every change: New / Improved / Fixed / Deprecated — breaking changes always lead
- **Writes per-audience variants** where meanings diverge: the same change reads differently to an admin, an end user, and a developer
- **Enforces the voice**: what changed and why it matters, plain verbs, present tense, no marketing adjectives, no exclamation points
- **Matches your terminology** — feed it past notes or a glossary and it follows your docs' vocabulary
- **Bounces ambiguity back**: "improved sync performance" returns as a question to engineering, not a guess in front of customers
- **Channel variants on request**: changelog, customer email, in-app announcement — same facts, different compression

## Why the ambiguity rule matters

A wrong release note is a support-ticket generator. The skill's core discipline is refusing to publish behavior the source notes don't establish — the questions list it returns is engineering's five-minute task, and it is cheaper than a week of confused customers.

## When it triggers

Phrases like:

- "Write release notes from these eng notes"
- "Turn these tickets into a changelog"
- "Draft the launch comms for this feature"
- "Admin notes and end-user notes for this release"

## Installation

### Option A — Install the skill folder (Claude Code)

Copy the skill folder into your Claude skills directory:

```bash
# Personal (all projects)
cp -r release-notes-skill ~/.claude/skills/

# Or project-scoped
cp -r release-notes-skill /path/to/project/.claude/skills/
```

Restart Claude Code (or start a new session) and the skill will be available.

### Option B — Use the packaged `.skill` file

Download [`release-notes-skill.skill`](./release-notes-skill.skill) and upload it wherever packaged skills are accepted (e.g. Claude.ai skill upload).

## Usage

Paste the raw notes and name the audience:

> Write release notes from these eng notes. Audiences: admins and end users. Past notes for voice: [paste or attach].

See [`examples/`](./examples) for a worked input and output (invented, illustrative data), including an ambiguous item bounced back as a question.

## Repository contents

- [`release-notes-skill/SKILL.md`](./release-notes-skill/SKILL.md) — the skill
- [`examples/`](./examples) — worked example (illustrative, invented data)
- [`release-notes-skill.skill`](./release-notes-skill.skill) — packaged for upload

## Part of the PMM Skill Stack

One of four free Claude Skills for product marketers: [cmoconfessions.com/skills](https://www.cmoconfessions.com/skills). Built by [Daniel Glickman](https://www.cmoconfessions.com) — product marketing and AI leader.
