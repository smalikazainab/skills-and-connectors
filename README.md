# Skills & Connectors — Lecture 8 Assignment

**Student Name:** Syeda Malika Zainab Kazmi
**AI Tools Used:** Claude.ai (skill-creator skill, Gmail Connector)
**Course:** The AI Agent Factory — Skills & Connectors Crash Course

## Summary

This repository contains five hands-on projects from the Skills & Connectors crash course: building a reusable Skill, connecting an app in a read-only way, combining a Skill with a Connector, proving the Skill is portable/shareable, and auditing an official Skill for safety.

---

## Task 1 — Build Your First Real Skill (Flashcard Maker)

**What it does:** A Skill that generates study flashcards (Question–Answer format) for any topic name, without needing notes as input.

**Prompt used:** `make flashcards on [topic]`

**Folder:** [`task-1-my-skill/`](./task-1-my-skill)

---

## Task 2 — Connect One App, Read-Only (Gmail)

**What it does:** Connected Gmail with read-only access and retrieved real email data through the connector.

**Prompt used:** `summarize my most recent email`

**Folder:** [`task-2-connect-app/`](./task-2-connect-app)

---

## Task 3 — Wire Skill + Connector Together

**What it does:** Combined the Task 1 Flashcard Skill with the Task 2 Gmail Connector in a single sentence — the Connector fetched live email content and the Skill formatted it into flashcards automatically.

**Prompt used:** `pull the content from my latest email and make flashcards from it`

**Folder:** [`task-3-skill-plus-connector/`](./task-3-skill-plus-connector)

---

## Task 4 — Hand Off

**What it does:** Shared the packaged Flashcard Maker skill file with a friend, who used it independently — with no explanation from me — and got a correctly formatted result.

**Prompt used (by my friend, independently):** `make flashcard on topic: Impacts of AI on jobs`

**Folder:** [`task-4-portable-handoff/`](./task-4-portable-handoff)

---

## Task 5 — Audit a Skill Before Trusting It

**What it does:** Installed and audited Anthropic's official `pdf` Skill — explained what it does in plain English, checked for external server contact, credential handling, and unexpected data transmission.

**Verdict:** ✅ Safe to enable — no network activity, no credential leakage, no unexpected data handling found.

**Folder:** [`task-5-skill-audit/`](./task-5-skill-audit)

---

