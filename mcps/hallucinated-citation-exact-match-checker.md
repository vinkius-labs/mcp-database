# Hallucinated Citation Exact Match Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hallucinated-citation-exact-match-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reliability](../categories/reliability.md)

Mathematically verify LLM quotes against ground-truth RAG context to detect fabrications.

## Description
This MCP server provides precision tools for verifying the factual integrity of LLM-generated citations. By performing deterministic character-level comparisons, it identifies exactly where a generated quote deviates from the provided source text. Use `verify_quote_integrity` to calculate match percentages and hallucination scores, `analyze_mismatch_locations` to find specific character offsets of errors, and `calculate_citation_validity` to receive categorical reliability ratings like 'Valid' or 'Hallucinated'. It is an essential bridge for developers building high-precision RAG systems that require mathematical certainty in citation accuracy.


## Available Tools (3)
- **analyze_mismatch_locations**: Identifies exactly where the LLM's text deviates from the provided truth
- **calculate_citation_validity**: Provides a high-level assessment of a citation's reliability based on both content and placement
- **verify_quote_integrity**: Determines if a specific quote is a faithful representation of the source text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hallucinated Citation Exact Match Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify if this quote is accurate: 'The sky is blue' from the source 'The sky is very blue.'"

**🤖 AI Agent:**
> The quote is a Partial match. The generated text deviates from the source text.

---

**👤 You:**
> "Check the integrity of the quote 'The sun is hot' against the source 'The sun is hot.'"

**🤖 AI Agent:**
> The quote is a Verbatim match with 100% integrity.

---

**👤 You:**
> "Is the citation 'The moon is cheese' valid for the source 'The moon is made of rock'?"

**🤖 AI Agent:**
> The citation is Hallucinated.


## ❓ FAQ

**Q: How does the tool detect hallucinations?**
The tool uses Levenshtein distance and longest common substring algorithms to calculate a hallucination score based on character deviation from the ground truth.

**Q: Can I see exactly where a quote is wrong?**
Yes, by using `analyze_mismatch_locations`, you receive a list of character offsets indicating exactly where the generated text diverges from the source.

**Q: What is a 'Valid' citation according to this tool?**
A citation is rated as 'Valid' when the `verify_quote_integrity` tool returns a 100% verbatim match.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hallucinated-citation-exact-match-checker](https://vinkius.com/mcp/hallucinated-citation-exact-match-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hallucinated Citation Exact Match Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hallucinated-citation-exact-match-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hallucinated Citation Exact Match Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hallucinated-citation-exact-match-checker": {
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
