# WCAG.com Accessibility MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wcagcom-accessibility)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wcagcom-accessibility-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wcagcom-accessibility-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Audit web accessibility — check compliance and guidelines via AI.

## Description
Empower your AI agent to orchestrate your entire web accessibility and inclusive design workflow with **WCAG.com**, the authoritative source for digital compliance data. By connecting the WCAG.com API to your agent, you transform complex accessibility audits into a natural conversation. Your agent can instantly analyze URLs for WCAG 2.1 compliance, audit specific issues and levels, and retrieve detailed remediation metadata without you ever touching a technical validator. Whether you are conducting quality assurance research or managing regional accessibility constraints, your agent acts as a real-time inclusive design consultant, ensuring your data is always verified and precise.

### What you can do

- **Accessibility Auditing** — Retrieve high-resolution reports for any URL, identifying issues and maintain a clear view of WCAG compliance.
- **Guideline Oversight** — Audit specific WCAG guidelines to understand the technical reach of your digital products instantly.
- **Issue Discovery** — Search for accessibility rules and standards to identify relevant stylistic markers for your UI components.
- **Metadata Intelligence** — Retrieve unique issue identifiers and remediation recommendations to assist in deep-dive classification.
- **Operational Monitoring** — Check API status to ensure your accessibility research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your WCAG.com API Key
3. Start managing your accessibility intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers & Designers** — monitor site accessibility and retrieve official metadata straight from your workflow.
- **Compliance Officers & QA** — verify WCAG standards and audit issue patterns without manual searching.
- **Accessibility Consultants** — perform rapid audits of client sites and identify relevant compliance markers through natural language.
- **Operations Leads** — automate design data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **audit_url_accessibility**: 1 standards to identify accessibility issues and compliance markers.

Perform a WCAG accessibility audit on a specific URL
- **check_api_status**: com Accessibility API.

Check if the WCAG.com service is operational
- **get_wcag_guideline_details**: Get detailed metadata and recommendations for a specific WCAG guideline
- **list_accessibility_rules**: List all accessibility rules used by the WCAG auditing engine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WCAG.com Accessibility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Perform an accessibility audit on 'https://example.com' using WCAG.com."

**🤖 AI Agent:**
> I've completed the accessibility audit for example.com! I've identified 12 issues, including 5 at the AA level related to color contrast and text scaling. Would you like the full issue list or specific remediation metadata for these findings?

---

**👤 You:**
> "What are the requirements for WCAG guideline '1.1.1'?"

**🤖 AI Agent:**
> I've retrieved the details for WCAG 1.1.1 (Non-text Content)! It requires all non-text content to have a text alternative that serves the equivalent purpose. I can provide the implementation recommendations and success criteria for this guideline.

---

**👤 You:**
> "List all accessibility rules used by the engine."

**🤖 AI Agent:**
> I've retrieved the full catalog of accessibility rules! They cover standards for perceivability, operability, and robustness. I can assist you with an audit of specific rule categories to help you identify relevant markers for your project.


## Installation & Usage

To install and use the **WCAG.com Accessibility** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wcagcom-accessibility](https://vinkius.com/mcp/wcagcom-accessibility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
