# Code Clone Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/code-clone-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Identifies duplicate or highly similar code blocks within a project using AST normalization and deterministic hashing.

## Description
The Code Clone Detector identifies identical and structurally similar code blocks within your codebase to prevent logic duplication. By utilizing AST Normalization, the system strips comments and whitespace while anonymizing identifiers (e.g., renaming variables to `v1`, `v2`). It uses Deterministic Hashing to find exact matches via `find_exact_clones` and calculates Levenshtein Distance for near-misses using `find_near_clones`. You can also assess technical debt with `calculate_duplication_metrics` to see the duplication percentage across your files.


## Available Tools (3)
- **calculate_duplication_metrics**: Provides a quantitative overview of redundancy within the analyzed files
- **find_exact_clones**: Identifies clusters of code that are functionally and structurally identical after normalization
- **find_near_clones**: Identifies code blocks that are structurally similar but contain slight variations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Code Clone Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all exact code clones in these files: ['src/index.ts', 'src/utils.ts']"

**🤖 AI Agent:**
> { "exactMatches": [ { "clusterId": "cluster-123", "occurrences": [ { "path": "src/index.ts", "lineRanges": ["10-25"] }, { "path": "src/utils.ts", "lineRanges": ["5-20"] } ] } ] }

---

**👤 You:**
> "Check for near-matches in 'src/logic.ts' with a similarity threshold of 0.8."

**🤖 AI Agent:**
> { "nearMatches": [ { "originalFile": "src/logic.ts", "cloneFile": "src/helper.ts", "similarityScore": 0.85 } ] }

---

**👤 You:**
> "What is the duplication percentage for the files in 'src/components/'?"

**🤖 AI Agent:**
> { "duplicationPercentage": 12.5, "totalLinesAnalyzed": 1500, "redundantLinesDetected": 187.5 }


## ❓ FAQ

**Q: How does the tool identify exact duplicates?**
The `find_exact_clones` tool uses AST Normalization to strip non-functional elements and then applies Deterministic Hashing to identify identical subtrees.

**Q: Can I detect code that is similar but not identical?**
Yes, the `find_near_clones` tool calculates the Levenshtein Distance between normalized code strings to find pairs with high structural similarity.

**Q: What metrics does the system provide?**
Using `calculate_duplication_metrics`, you can obtain the duplication percentage, total lines analyzed, and the number of redundant lines detected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/code-clone-detector](https://vinkius.com/mcp/code-clone-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Code Clone Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `code-clone-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Code Clone Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "code-clone-detector": {
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
