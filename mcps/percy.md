# Percy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/percy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Execute visual regression tests via Percy — track visual diffs natively, inspect snapshot limits, approve builds, and verify UI components using AI.

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


## Available Tools (10)
- **list_builds**: List builds for a Percy project. Each build contains snapshots from a test run. Returns build IDs, states (processing/finished/failed), branch names, commit SHAs, and snapshot counts
- **get_build_details**: Get full details of a Percy build including state, total/unreviewed snapshot counts, approved/rejected snapshots, branch, commit SHA, and finalized timestamp
- **approve_build**: /approve` moving the test suite to green.

Approve all unreviewed snapshots in a Percy build. Marks the entire build as visually approved for deployment
- **list_projects**: List all projects on Percy (BrowserStack). Percy is the leading visual regression testing platform that captures snapshots and detects pixel-level UI differences across builds. Uses JSON:API format. Returns project names, slugs, and browser configs
- **get_project_details**: Get full details of a Percy project including name, slug, default branch, auto-approve enabled, browser targets, and build count
- **list_snapshots**: List snapshots in a Percy build. Each snapshot is a captured page/component at specific widths and browsers. Returns snapshot names, review states (unreviewed/approved/rejected), and diff percentages
- **get_snapshot_details**: Get full details of a Percy snapshot including name, review state, widths, fingerprint, and comparison count
- **approve_snapshot**: Approve a single Percy snapshot. Marks it as visually correct, updating the baseline for future comparisons
- **list_comparisons**: List visual comparisons for a Percy snapshot. Each comparison shows the diff between baseline and head at a specific width/browser. Returns diff images, diff percentages, and browser info
- **list_browsers**: List all supported browser families on Percy. Returns browser names, versions, and OS combinations for cross-browser visual testing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Percy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Log explicitly the builds targeting structural limits seamlessly isolating project 'org-slug/my-app' dynamically checking bounding states natively."

**🤖 AI Agent:**
> Queried structured native limits logically hitting endpoints gracefully globally. Validated boundaries tracking 3 explicit recent builds logically seamlessly natively. Top bound is Build ID 9091x running structurally 'unreviewed' accurately completely actively globally.

---

**👤 You:**
> "Reverse check explicit structures extracting limits comparing properties cleanly bounding snapshot ID 'snap_778' natively efficiently."

**🤖 AI Agent:**
> Mapped explicit target bounds successfully routing API queries globally resolving gracefully testing results gracefully efficiently. Captured snapshot limits natively show structural bounds identifying a 3.2% exact diff regression rendering gracefully explicitly locally tracking arrays.

---

**👤 You:**
> "Force explicit validation mutating boundaries executing structurally an approval across build ID '8910' automatically natively flawlessly securely."

**🤖 AI Agent:**
> Dispatched JSON gracefully natively mutating endpoint execution safely actively explicitly properly mapping target specifications limits. Build '8910' structurally updated effectively generating bounding approval. Pipeline logic seamlessly gracefully confirmed natively securely correctly completely logically active.


## ❓ FAQ

**Q: Can the AI automatically approve an entire Percy build limit safely via constraints natively?**
Absolutely strictly explicitly natively. The integration encapsulates the `approve_build` action dynamically structurally executing the final endpoint verification marking bounds explicitly matching visual approvals effortlessly saving limits.

**Q: How explicitly strict are the parameter bounds when extracting image comparisons logistically?**
Invoking Explicit bounding via `list_comparisons` tracks native image differences safely cleanly bounding metrics returning explicit difference percentages mapping base width loops directly over testing node grids explicitly gracefully natively.

**Q: Where structurally globally do I find my Explicit Percy integration token accurately gracefully?**
Navigate explicit bounds inside your native Percy workspace parameters explicitly mapping 'Project Settings > Integrations/Tokens'. Globally limit testing node arrays explicitly generating Token strings seamlessly securely correctly internally securely elegantly here.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/percy](https://vinkius.com/mcp/percy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Percy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `percy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Percy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "percy": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
