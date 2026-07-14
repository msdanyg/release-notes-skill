---
name: release-notes-skill
description: Turns raw engineering notes — tickets, PR descriptions, bullet points — into clean, audience-correct release notes and launch communications. Classifies every change (New, Improved, Fixed, Deprecated), writes separate variants where audiences diverge (admin, end user, developer), enforces a plain-verbs no-hype voice matched to the product's existing terminology, and bounces ambiguous items back as questions to engineering instead of guessing in front of customers. Produces changelog, customer-email, and in-app variants on request.
---

# Release Notes Skill

## What This Skill Does

Converts raw engineering output into release notes a reader can act on — sorted by what the change means for them, written for the audience each note serves, and honest about anything the source notes do not establish.

**Key capabilities:**
- Classifies every change: New / Improved / Fixed / Deprecated
- Writes per-audience variants where they diverge — admin, end user, developer
- Enforces the voice: what changed and why it matters, plain verbs, present tense, no marketing adjectives
- Matches the product's existing terminology (asks for a glossary or past notes to calibrate)
- Bounces ambiguous items back as questions to engineering — never guesses in front of customers
- Generates channel variants on request: changelog entry, customer email, in-app announcement

## When to Use This Skill

Use for any release, from a weekly changelog to a headline launch. Typical requests:

- "Write release notes from these eng notes"
- "Turn these tickets into a changelog"
- "Draft the launch comms for this feature"
- "Admin notes and end-user notes for this release"

## Required Inputs

1. **Raw feature notes** — tickets, PR descriptions, engineering bullets, in any state.
2. **The audience(s)** — admin, end user, developer, or several. If not specified, ask; the audience determines the note.
3. Optional but valuable: **past release notes or a glossary**, to match house voice and terminology.

## The Hard Rules

1. **Never announce behavior the notes do not establish.** "Improved sync performance" is not publishable — improved how, by how much, for whom? Ambiguity goes back to engineering as a question, not forward to customers as a guess. A wrong release note is a support-ticket generator.
2. **The audience determines the note.** The same change means different things to an admin (permissions, rollout, configuration), an end user (what they can now do), and a developer (contracts, breaking changes). Where meanings diverge, write separate notes; never blur them into one.
3. **Voice is enforced, not suggested.** Lead with what changed and why it matters to that reader. Plain verbs, present tense. No "exciting," no "we're thrilled," no exclamation points. Superlatives are banned; specifics are the substitute.
4. **Terminology follows the product's docs.** If the docs say "workspace," the notes never say "project." Ask for a reference if none was provided.
5. **Breaking changes lead.** Deprecations and breaking changes go first for the audiences they affect, with dates and required actions — never buried under features.

## Procedure

1. **Ingest and classify.** Sort every item: New / Improved / Fixed / Deprecated. Flag anything that is two changes bundled as one (split them).
2. **Resolve the audience map.** For each item, decide which audiences it touches and whether they need distinct notes.
3. **Separate the publishable from the ambiguous.** An item is publishable when the source establishes: what changed, who it affects, and any action required. Everything else goes to the questions list.
4. **Write the notes.** Per audience, ordered: breaking/deprecations first, then New, Improved, Fixed. Each note: what changed → why it matters to this reader → action required (if any). One to three sentences; a note that needs more is usually a doc, and the note should link to it.
5. **Run the voice pass.** Strip adjectives that assert quality instead of describing behavior. Verify terminology against the provided reference. Present tense throughout.
6. **Return the questions list.** Every ambiguous item, phrased as a specific question to engineering ("Sync performance — improved for initial sync, incremental, or both? Measured at what scale?").
7. **Offer channel variants.** On request: changelog entry (tersest), customer email (adds context and links), in-app announcement (one sentence plus a link). Same facts in every channel — only compression changes.

## Output Format

1. **Release notes**, grouped by audience, breaking changes first.
2. **Questions for engineering** — the ambiguous items (write "None — all items were publishable as supplied" if empty).
3. One closing line offering channel variants.

The test for every note: could the reader take the right action from this note alone? If not, it is not done.
