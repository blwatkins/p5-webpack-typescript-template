# CLAUDE.md

Guidance for Claude Code (and other AI assistants) when working in this repository.

## Canonical Instructions

The detailed, authoritative conventions for this project live in [`.github/copilot-instructions.md`](./.github/copilot-instructions.md).
Read that file before making any change to this repository, including documentation-only changes.
This document is a map of what lives there; it does not repeat its rules — the sync rule below is the deliberate exception, since an agent that opens only one of the two files still needs it.

## Keep These Two Files in Sync

This repository maintains both `CLAUDE.md` and `.github/copilot-instructions.md`.
`CLAUDE.md` is a map of where guidance lives; `.github/copilot-instructions.md` holds the guidance itself.
Add or change a convention in `.github/copilot-instructions.md`, not here.

This file carries two kinds of content: links into `.github/copilot-instructions.md`, and a small number of facts restated in its own words where a link would cost more than it saves.
Update this file when a change there invalidates either kind:

- **A link stops resolving** — a section this file links to is renamed, moved, or removed.
- **A restated fact stops matching** — a summary, a name, or a list spelled out here rather than linked no longer matches `.github/copilot-instructions.md`.

A new convention added under an existing section invalidates neither, and requires no change here.

A new *section* in `.github/copilot-instructions.md` is the one case that needs judgment, since it is not yet linked from anywhere.
Add it to the map only if a contributor would need to know the section exists before starting work; leave it off if they would find it by reading `.github/copilot-instructions.md` once they reach the work it governs.
When the call is close, leave this file alone — an incomplete map costs less than a map that drifts into a second copy.

## Project Summary

A template project for using p5.js with TypeScript and webpack.

## npm Commands

See the ["npm Scripts" section of `.github/copilot-instructions.md`](./.github/copilot-instructions.md#npm-scripts) for the full list of available commands.

## Generated Output Directories (not committed)

`_dist/` (build) and `_compiled/` (TypeScript `outDir`) are generated and gitignored.

## Documentation Notes

Documentation, the GitHub Pages site, and the portfolio skills page (`docs/portfolio-skills.md`) are governed by the ["Documentation and GitHub Pages"](./.github/copilot-instructions.md#documentation-and-github-pages) and ["Portfolio Page Generation and Maintenance"](./.github/copilot-instructions.md#portfolio-page-generation-and-maintenance) sections of `.github/copilot-instructions.md`.

Markdown indentation rules for all repository `.md` files are in the ["Markdown Formatting" section of `.github/copilot-instructions.md`](./.github/copilot-instructions.md#markdown-formatting).

## Pre-Merge and Release Review

Before merging a branch, complete these review steps (full details in the ["Pre-Merge and Release Review" section of `.github/copilot-instructions.md`](./.github/copilot-instructions.md#pre-merge-and-release-review)):

1. **Validation** — `npm ci`, then `npm run validate` (lint and build) passes cleanly
2. **Portfolio skills page** — review `docs/portfolio-skills.md` for accuracy and currency, per the linked section
3. **Instruction file sync** — `CLAUDE.md` and `.github/copilot-instructions.md` are consistent and current
4. **Branch code review** — convention compliance, code quality, and cross-source consistency, per the linked section
