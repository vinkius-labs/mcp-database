# Google Lighthouse SEO Auditor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-lighthouse-seo-auditor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-lighthouse-seo-auditor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-lighthouse-seo-auditor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Transform your AI into a Technical SEO & Performance Agency. Instantly run official Google PageSpeed Insights (Lighthouse) audits on any website and get exact code fixes to achieve a perfect 100/100 score.

## Description
Stop paying agencies thousands of dollars for performance audits. This MCP connects your AI agent directly to the official **Google PageSpeed Insights API**, turning it into an elite Technical SEO and Frontend expert.

### The Superpowers

- **Instant Competitor Analysis:** Ask the AI to audit a competitor's website. It will run a full Lighthouse scan (Mobile or Desktop) and return their exact scores for Performance, Accessibility, Best Practices, and SEO.
- **Actionable Code Fixes:** Unlike a normal dashboard that just tells you "Render-blocking resources found", the AI reads the specific failing audits and writes the exact React, Next.js, or HTML code you need to copy/paste to fix it.
- **Zero Friction:** No authentication required for standard use. Just connect the MCP and start auditing websites immediately. Your AI agent can now visually optimize web applications on the fly.


## Available Tools
- **run_lighthouse_audit**: Returns the scores (0-100) and specific failed audits (e.g. large images, render-blocking JS) so you can suggest exact code fixes.

Runs a full Google PageSpeed Insights (Lighthouse) audit on any public URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Lighthouse SEO Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit the performance of https://vinkius.com on mobile and tell me how to get to 100/100."

**🤖 AI Agent:**
> I've ran the Lighthouse audit. **Scores:** Performance: 72, Accessibility: 95, SEO: 100.

The main issue dragging your Performance down is a **Render-blocking resource** (`main.js` taking 1.2s to load). 
To fix this, add the `defer` attribute to your script tag. I will update your `index.html` file now to implement this change.

---

**👤 You:**
> "Run an accessibility audit on https://github.com to see if they missed anything."

**🤖 AI Agent:**
> I audited GitHub's homepage. They scored **100/100 on Accessibility**. However, the Best Practices score is 83/100 because of an issue with a third-party cookie missing the `SameSite` attribute. As developers, we can learn from their flawless ARIA role implementation.


## Installation & Usage

To install and use the **Google Lighthouse SEO Auditor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-lighthouse-seo-auditor](https://vinkius.com/mcp/google-lighthouse-seo-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
