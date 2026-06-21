# Percy MCP Server

Execute visual regression tests via Percy — track visual diffs natively, inspect snapshot limits, approve builds, and verify UI components using AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/percy)

## Overview
**Category:** ship-it
**Tools Count:** 10

## Description
Inject precision quality assurance workflows directly bounding LLM models via the **Percy Visual Testing API** (by BrowserStack). Programmatically verify pixel regressions executing queries evaluating visual boundaries natively across target projects. Inspect deep status arrays parsing CI build limits dynamically, extract metrics evaluating granular snapshot checkpoints asynchronously, and force immediate test baseline approvals seamlessly directly from explicit prompt commands naturally.

### What you can do

- **Project Navigation** — Read bounded parameters tracking Percy deployments isolating configurations determining explicitly specific active QA targets natively
- **Automated Build Oversight** — Track specific arrays extracting dynamic checks returning pipeline checkpoints (approved/failed/unreviewed limits) explicitly seamlessly
- **Visual Snapshot Operations** — Log natively extracting bounds verifying comparison properties logging rendering differences mapping exact explicit width constraints
- **Baseline Affirmations** — Mutate bounding loops forcing active execution of JSON logic structurally bypassing native clicks allowing test approvals implicitly (`approve_build` or `approve_snapshot`)

### How it works

1. Enable the structural node mapping target locally inside your logic constraints securely
2. Incorporate explicitly bounds adding your single Percy Project Token statically internally gracefully
3. Engage conversational agents dynamically explicitly retrieving UI test results bounding seamlessly

### Who is this for?

- **QA & Testing Engineers** — extract specific arrays parsing failed assertions tracking structural rendering regressions safely returning granular boundaries immediately iteratively
- **Frontend Teams** — resolve visual bounds logging pipeline limits running explicitly without traversing complex dashboards isolating errors easily intelligently natively
- **DevOps Admins** — verify explicit pipeline health tracking CI loop states explicitly monitoring unreviewed elements globally reliably securely


## Available Tools
- **list_projects**: List all projects on Percy (BrowserStack). Percy is the leading visual regression testing platform that captures snapshots and detects pixel-level UI differences across builds. Uses JSON:API format. Returns project names, slugs, and browser configs
- **get_project_details**: Get full details of a Percy project including name, slug, default branch, auto-approve enabled, browser targets, and build count
- **list_builds**: List builds for a Percy project. Each build contains snapshots from a test run. Returns build IDs, states (processing/finished/failed), branch names, commit SHAs, and snapshot counts
- **get_build_details**: Get full details of a Percy build including state, total/unreviewed snapshot counts, approved/rejected snapshots, branch, commit SHA, and finalized timestamp
- **approve_build**: /approve` moving the test suite to green.

Approve all unreviewed snapshots in a Percy build. Marks the entire build as visually approved for deployment
- **list_snapshots**: List snapshots in a Percy build. Each snapshot is a captured page/component at specific widths and browsers. Returns snapshot names, review states (unreviewed/approved/rejected), and diff percentages
- **get_snapshot_details**: Get full details of a Percy snapshot including name, review state, widths, fingerprint, and comparison count
- **approve_snapshot**: Approve a single Percy snapshot. Marks it as visually correct, updating the baseline for future comparisons
- **list_comparisons**: List visual comparisons for a Percy snapshot. Each comparison shows the diff between baseline and head at a specific width/browser. Returns diff images, diff percentages, and browser info
- **list_browsers**: List all supported browser families on Percy. Returns browser names, versions, and OS combinations for cross-browser visual testing


## Installation & Usage

To install and use the **Percy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/percy](https://vinkius.com/mcp/percy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
