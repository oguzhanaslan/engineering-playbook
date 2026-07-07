<div align="center">

# Engineering Playbook

**A lightweight, token-efficient Claude Code toolkit for engineering leaders who build, review, and ship.**

[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)](#)
[![Format](https://img.shields.io/badge/format-Markdown-blue.svg)](#)
[![Built for](https://img.shields.io/badge/built%20for-Claude%20Code-8A2BE2.svg)](https://docs.claude.com/en/docs/claude-code)
[![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](#license)

</div>

---

## Table of Contents

- [Overview](#overview)
- [Key Topics](#key-topics)
- [Structure](#structure)
- [Skills](#skills)
- [Usage](#usage)
- [Design Principles](#design-principles)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

A minimal, modular set of Claude Code **skills** that turn Claude into a reliable pair for daily engineering work — from merge-request reviews to ADRs — while keeping context small and answers sharp.

- **Lightweight** — every file is short and single-purpose.
- **Token-efficient** — references and templates load only when a skill needs them.
- **Practical** — checklist-first outputs you can act on immediately.

## Key Topics

| Topic | What it covers |
|---|---|
| **Code Standards** | Reusable rules for clean, testable, review-ready changes. |
| **Code Review** | Actionable MR comments with severity and suggested fixes. |
| **Architecture & Decisions** | Option analysis, trade-offs, and one-page ADRs. |
| **Leadership** | Reusable principles for clarity, feedback, and team throughput. |

## Structure

- `.claude/CLAUDE.md` — minimal base config Claude loads first.
- `.claude/skills/` — one folder per skill, each with a `SKILL.md`.
  - `references/` — reusable standards, loaded only when quality rules are needed.
  - `templates/` — copy-paste output shapes, loaded only when producing an artifact.

## Skills

| Skill | Use it when |
|---|---|
| `review` | Reviewing merge requests, diffs, or source code |
| `implement` | Making small, focused code changes |
| `docs` | Writing or updating engineering documentation |
| `jira` | Drafting Jira tasks and acceptance criteria |
| `investigate` | Tracing data flow and root-cause analysis |
| `architecture` | Evaluating design options and trade-offs |
| `decision` | Writing Architecture Decision Records |
| `meeting` | Turning meetings into decisions and actions |
| `leadership` | Leadership communication and management notes |

## Usage

1. Copy `.claude/` into your project (or point Claude Code at this repo).
2. Skills are selected two ways:
   - **Automatically** — Claude matches your request to a skill's `description`.
   - **Intentionally** — phrase the task to target one (e.g. "review this MR", "write an ADR").
3. Each skill pulls only the reference or template it needs — nothing more.

## Design Principles

- **Single source per rule** — no duplicated instructions.
- **References over duplication** — skills point to references and templates.
- **Checklist-first** — concise, scannable, actionable output.
- **Execution-optimized** — tuned for Claude Code efficiency, not just human reading.

## Contributing

Contributions are welcome. Keep changes small, single-purpose, and token-efficient — the same standards this playbook promotes.

## License

Released under the MIT License. Feel free to explore, adapt, and build on it.
