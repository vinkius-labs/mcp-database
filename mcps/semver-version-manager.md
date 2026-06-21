# SemVer Version Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semver-version-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop LLMs from guessing software versions. Deterministically evaluate semantic version bounds, compatibilities, and sort releases perfectly.

## Description
LLMs hallucinate software versions. They constantly fail to evaluate complex semantic version boundaries (like `>=1.4.0 <2.0.0`) and often suggest broken dependency resolutions. This native MCP offloads all version math to the official NPM SemVer engine.

### The Superpowers

- **Absolute Determinism:** Let the AI parse package.json files and offload the actual compatibility checks to this engine. No more broken builds due to hallucinated version logic.
- **Lightning Fast Sorting:** Pass an array of 50 disorganized software versions and get a perfectly sorted semantic list back in milliseconds.
- **Zero Dependency Hell:** Runs natively on the edge. By preventing AI from guessing version bumps, your automated CI/CD agents become mathematically perfect.


## Available Tools
- **check_semver_compatibility**: Checks if a specific version satisfies a SemVer range (e.g. ^1.4.2)
- **sort_semver_list**: Pass both versions and receive the comparison result (greater, lesser, equal). Essential for dependency resolution.

Sorts a JSON array of version strings correctly following semantic versioning rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SemVer Version Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify deterministically if version `2.4.1` satisfies the peer dependency range `^2.0.0`."

**🤖 AI Agent:**
> ✅ **SemVer Result:** Satisfied. `2.4.1` is safely within the `^2.0.0` caret constraints.

---

**👤 You:**
> "Sort this array of 12 release tags (including `-rc.1` and `-beta`) in descending order."

**🤖 AI Agent:**
> ✅ **Sorted Order:**
1. `v2.0.0`
2. `v2.0.0-rc.1`
3. `v2.0.0-beta.2`
...

---

**👤 You:**
> "What is the result of applying a 'minor' bump to version `1.4.3-alpha`?"

**🤖 AI Agent:**
> ✅ **New Version:** `1.5.0`. The alpha pre-release tag is dropped during a standard minor bump.


## ❓ FAQ

**Q: Why use this instead of letting the LLM read the version?**
LLMs do not understand numerical boundaries logically.

**Q: Does it support pre-release tags?**
Yes, it perfectly evaluates -alpha, -beta, and -rc tags according to SemVer rules.

**Q: Can it sort an array of versions?**
Yes, passing an array guarantees a flawless descending or ascending output.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semver-version-manager](https://vinkius.com/mcp/semver-version-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SemVer Version Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `semver-version-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SemVer Version Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "semver-version-manager": {
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
