# Image SEO Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/image-seo-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Automated analysis of image metadata to identify SEO and accessibility violations.

## Description
The Image SEO Auditor provides a specialized toolkit for evaluating the health of your web assets. Using `inspect_single_image`, you can break down specific violations like generic filenames or excessive file sizes. For larger collections, `audit_image_set` generates high-level summaries and detailed reports across entire image sets. Additionally, `fetch_audit_guidelines` allows you to retrieve the exact thresholds used for scoring, ensuring your optimization strategy aligns with current best practices.


## Available Tools (3)
- **audit_image_set**: Perform a bulk SEO analysis on a collection of images
- **fetch_audit_guidelines**: Retrieve the current SEO audit thresholds and patterns
- **inspect_single_image**: Analyze a single image for SEO and accessibility violations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Image SEO Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this image for SEO issues: filename is 'hero.jpg', alt text is '', and size is 500KB."

**🤖 AI Agent:**
> The image 'hero.jpg' has a score of 60 (MEDIUM_RISK). Violations detected: Empty alt text and file size exceeds the recommended threshold.

---

**👤 You:**
> "Audit this set of images: [{'filename': 'product.png', 'altText': 'Blue running shoes', 'fileSizeKb': 45}, {'filename': 'image001.jpg', 'altText': '', 'fileSizeKb': 1200}]"

**🤖 AI Agent:**
> Audit complete. Average Score: 80. Total Processed: 2. Critical Violations: 1. Summary: 'product.png' is optimized, while 'image001.jpg' failed due to generic naming and excessive size.

---

**👤 You:**
> "What are the current file size limits for a good SEO score?"

**🤖 AI Agent:**
> The current maximum recommended size threshold is 200KB.


## ❓ FAQ

**Q: How does the auditor determine if a filename is generic?**
The tool checks filenames against common generic patterns such as 'image001.jpg', 'IMG_', or 'DSC_'. You can see the full list of patterns by using `fetch_audit_guidelines`.

**Q: Can I audit multiple images at once?**
Yes, use the `audit_image_set` tool by providing a JSON array of image objects containing filenames, alt text, and file sizes.

**Q: What criteria are used for the SEO score?**
The score is calculated based on three pillars: presence of descriptive alt text, avoidance of generic filenames, and keeping file sizes below the recommended threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/image-seo-auditor](https://vinkius.com/mcp/image-seo-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Image SEO Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `image-seo-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Image SEO Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "image-seo-auditor": {
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
