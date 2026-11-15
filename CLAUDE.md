# CLAUDE.md

This file provides guidance to AI assistants working in this repository.

## Project Purpose

A library of Claude skills distilled from studying creators' methods (no application code). Skill content is written in Italian; industry terms (CPL, VSL, ad set, CAPI…) stay in English.

## Directory Layout

- `.claude/skills/<name>/SKILL.md`: one skill per folder, loaded automatically by Claude Code in this repo
- `.claude/skills/<name>/references/`: detail files the SKILL.md points to (progressive disclosure)
- `.claude/skills/<name>/evals/`: test cases in the `claude plugin eval` layout (`prompt.md`, `case.yaml`, `graders/`); excluded from packaging
- `dist/<name>.skill`: packaged skill for upload to claude.ai (zip of the skill folder, without `evals/`)

Current skills:

- `revel-meta-leadgen`: Revel Loughlin's Meta Ads lead generation method, from 5 videos (Sep 2025 - Nov 2026); sources listed in `references/fonti-e-casi-studio.md`
- `modular-video-ads-system`: v2 of the owner's own modular video ads system (synced from claude.ai and upgraded here; keep the same name so the package replaces the original). Adds concept-first design for Andromeda, Hormozi's body/CTA grid, optional objection and pretext modules, and an internal launch/test protocol

Research notes (full-transcript studies, Italian) live in `ricerca/`: `hormozi-ads-leadgen-note.md` and `sam-piliero-meta-ads-note.md`.

## Context About the Owner: Look It Up, Never Ask

The owner does not want questions about things that can be looked up. Before asking anything about their business, clients, preferences or history, search these sources, and state what you found instead of asking:

- Synced claude.ai skills under `~/.claude/skills/synced/*/`, notably `stoic-second-brain` (map of the Notion second brain), `mentore-totale-giuseppe/references/profilo_completo.md`, `modular-video-ads-system/references/examples.md`, `business-architect`, `hormozi-100m-offers`
- The Notion second brain via the Notion connector: the Areas database (Type = Clients) and the CRM database (Status = Client). The two are not fully in sync, so cross-check both
- `vault_context` / `vault_write`, when those tools are available in the session

Never infer a client's country from the language of their ads; check the CRM record.

## Conventions

- Skill names are kebab-case; the `description` frontmatter must stay under 1024 characters and contain no angle brackets
- Keep SKILL.md under ~500 lines; push detail into `references/`
- Mark interpretations that are not the creator's own words, and keep a "Lacune" (gaps) list of what has not been studied yet
- After editing a skill, re-validate and re-package it with the skill-creator scripts (`quick_validate`, `package_skill`)
- Never use em dashes or en dashes in any content (the owner's fixed preference): use a normal hyphen, colon or comma

## Git Workflow

- Default branch: `main`
- Feature work goes on short-lived branches off `main`
- Commit messages: imperative mood, present tense (e.g. "Add login endpoint")
- Keep commits focused: one logical change per commit

## Working with Claude Code

- Run `claude` in the repo root to start an interactive session
- Use `/help` for a list of available slash commands
- CLAUDE.md is read automatically at session start; keep it up to date as the project evolves
- Prefer editing existing files over creating new ones unless a new file is clearly needed
- Do not add comments that merely restate what the code does; only note non-obvious constraints or workarounds
