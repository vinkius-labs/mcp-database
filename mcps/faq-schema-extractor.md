# FAQ Schema Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faq-schema-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Automatically identify Q&A pairs from unstructured text and generate SEO-ready JSON-LD FAQPage schema.

## Description
The FAQ Schema Extractor is a specialized tool designed to transform unstructured, human-readable prose into machine-readable structured data. By using the `extract_pairs` tool, you can identify individual question and answer pairs from any block of text. Once extracted, the `generate_jsonld` tool wraps these pairs into a valid JSON-LD format following Schema.org standards. Finally, use `validate_schema_integrity` to ensure your generated script is syntactically correct and safe for production deployment in your website's head section.


## Available Tools (3)
- **extract_pairs**: Extracts Q&A pairs from unstructured text
- **generate_jsonld**: Generates JSON-LD FAQPage schema
- **validate_schema_integrity**: Validates JSON-LD schema integrity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FAQ Schema Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract pairs from this text: Q: What is MCP? A: Model Context Protocol. Q: Is it free? A: Yes."

**🤖 AI Agent:**
> [{"question": "What is MCP?", "answer": "Model Context Protocol."}, {"question": "Is it free?", "answer": "Yes."}]

---

**👤 You:**
> "Generate JSON-LD from these pairs: [{"question": "Who are you?", "answer": "I am an AI assistant."}]"

**🤖 AI Agent:**
> <script type="application/ld+json">{"@context": "https://schema.org", "@type": "FAQPage", "mainEntity": [{"@type": "Question", "name": "Who are you?", "acceptedAnswer": {"@type": "Answer", "text": "I am an AI assistant."}}]}</script>

---

**👤 You:**
> "Validate this JSON-LD: <script type="application/ld+json">{"@context": "https://schema.org", "@type": "FAQPage"}</script>"

**🤖 AI Agent:**
> {"isValid": true, "validationIssues": []}


## ❓ FAQ

**Q: How do I start extracting Q&A pairs?**
Use the `extract_pairs` tool by providing your raw text in the `rawText` parameter. You can choose between pattern recognition or block separation modes.

**Q: What format is the output JSON-LD in?**
The `generate_jsonld` tool produces a complete `<script type="application/ld+json">` block that is ready to be pasted directly into the HTML head of your webpage.

**Q: How can I ensure my schema is valid for Google?**
After generating your JSON-LD, run it through the `validate_schema_integrity` tool to check for syntax errors or missing mandatory Schema.org fields.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faq-schema-extractor](https://vinkius.com/mcp/faq-schema-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FAQ Schema Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `faq-schema-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FAQ Schema Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "faq-schema-extractor": {
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
