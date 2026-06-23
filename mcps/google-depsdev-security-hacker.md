# Google Deps.dev Security Hacker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-depsdev-security-hacker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Transform your AI into a Senior DevSecOps Engineer. Instantly audit any open-source package, hunt for hidden supply-chain threats in dependency trees, and analyze full GitHub repositories using Google's deps.dev API. No authentication required.

## Description
Equip your AI agent with the ultimate "Hacker" toolkit for open-source security. This MCP connects your agent directly to Google's Open Source Insights (deps.dev), turning it into a specialized DevSecOps auditor capable of uncovering deep vulnerabilities that basic scanners miss.

### The 4 Superpowers

- **1. Instant Vulnerability Audits:** Drop a package name into the chat and ask the AI to "Audit this dependency." It will instantly flag any library with known CVEs or GitHub Security Advisories.
- **2. Supply Chain Threat Hunting:** A package might look safe, but what about its dependencies? The AI can map the *entire transitive dependency tree* to find hidden malware or unpatched vulnerabilities lurking deep in the stack.
- **3. Repository Governance (OSSF):** Paste any GitHub URL and let the AI generate a full governance audit. It uses the OSSF Scorecard to check if the repository enforces code reviews, uses fuzzing, and signs its releases.
- **4. CVE Encyclopedia:** Give the AI any CVE or GHSA ID, and it will pull down the exact exploit details, severity, and the specific package versions affected so you can patch immediately.

Works natively with npm (Node.js), PyPI (Python), Cargo (Rust), Go, Maven (Java), and NuGet (.NET).


## Available Tools (4)
- **analyze_dependency**: Support systems: npm, pypi, go, cargo, maven, nuget.

Analyzes an open-source package for security advisories and OSSF scorecard using Google deps.dev
- **analyze_github_repository**: Performs a full security and governance audit of a GitHub repository using OSSF Scorecards
- **get_transitive_dependencies**: Hunts for hidden security threats by analyzing the entire transitive dependency tree of a package
- **get_vulnerability_details**: Retrieves detailed information about a specific CVE or GitHub Security Advisory (GHSA)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Deps.dev Security Hacker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit the npm package 'express' version 4.16.0 for any security vulnerabilities."

**🤖 AI Agent:**
> I checked `express` v4.16.0 on deps.dev. It has **4 known security advisories**, including GHSA-8X4W-MXXF-XXXX (High Severity - CVSS 7.5). The project has an OSSF Scorecard of 6.8/10. I strongly recommend upgrading.

---

**👤 You:**
> "I found this GHSA-xvch-5gv4-984h advisory. What does it do and what packages are affected?"

**🤖 AI Agent:**
> That ID corresponds to a **CRITICAL (CVSS: 9.8)** vulnerability: "Prototype Pollution in Lodash". It allows an attacker to inject properties into Object.prototype. It affects the npm package `lodash` on versions `< 4.17.15`. You must upgrade immediately.

---

**👤 You:**
> "Check the dependency tree for the pypi package 'requests' v2.28.1. Are there any hidden threats?"

**🤖 AI Agent:**
> I mapped the entire transitive tree (total 8 dependencies). **⚠️ WARNING: Found 1 hidden threat:** The indirect dependency `certifi` (v2022.6.15) has a known security advisory. You should override this dependency in your requirements.


## ❓ FAQ

**Q: Do I need an API key for this?**
No! The Google deps.dev API is completely free and public. Just connect the MCP and your AI agent can start auditing immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-depsdev-security-hacker](https://vinkius.com/mcp/google-depsdev-security-hacker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Deps.dev Security Hacker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-depsdev-security-hacker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Deps.dev Security Hacker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-depsdev-security-hacker": {
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
