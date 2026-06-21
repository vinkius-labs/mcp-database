# Veracode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/veracode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/veracode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/veracode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Bring Veracode AppSec to your AI. Analyze source code flaws, extract application profiles, and track vulnerabilities conversationaly.

## Description
Equip your AI agent with complete read and write access to your **Veracode** ecosystem. Seamlessly blend application security posture management alongside your typical development workflow using entirely conversational AI.

### What you can do

- **Unified Vulnerability Tracing** — Ask the agent to list Open security findings or mitigation statuses spanning across Static (SAST), Dynamic (DAST), and Component (SCA) analytics per application.
- **Deep Flaw Details** — Input specific Finding IDs and let the bot explain the underlying CWE error, affected code strings, severity ratings, and automated remediation tutorials.
- **Portfolio AppSec Management** — List tracked applications, create novel application profiles on the fly before a commit, or request health checks mapping sandbox testing environments.
- **Dynamic Scan Queries** — Poll your AI intuitively ensuring it retrieves the real-time execution bounds of your scheduled Web Application Security runtime scenarios.

### How it works

1. Subscribe to this connected server
2. Securely provide your dual Veracode API ID and API Secret pair
3. Engage directly with Claude, Cursor, or compatible clients querying security intelligence intuitively

### Who is this for?

- **DevSecOps Engineers** — bypass extensive console clicking to check scan statuses and manually export flaws by chatting internally for a summary.
- **Application Developers** — fix security defects natively in Cursor by commanding it to read the flawed line out of the Veracode finding ID report directly.
- **CISO & Security Managers** — audit all authenticated identity users or track general application risk matrices effortlessly reading human-summarized text outputs.


## Available Tools
- **create_application**: Provide the app schema and profile name as a JSON string.

Create a new Veracode application profile container
- **delete_application**: This action is irreversible.

Delete a Veracode application permanently
- **get_api_health**: Check the health of Veracode connection
- **get_application_details**: Information includes its Veracode compliance policy status, business criticality rating, deployment state, and risk scores.

Get a detailed profile of a Veracode application
- **get_finding_details**: Explains the vulnerability type (CWE), affected source file, code path, and remediation guidance.

Get precise vulnerability details for a specific flaw/finding
- **list_applications**: Most structural entities return a globally unique GUID which is required for sub-resource lookups.

List all Veracode AppSec Applications
- **list_dynamic_analyses**: List configured Dynamic Analysis (DAST) scans
- **list_security_findings**: Retrieve the unified security findings for an application
- **list_sandboxes**: List all testing sandboxes linked to an application
- **list_veracode_users**: Used to manage RBAC roles.

List authorized Veracode identity users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Veracode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications currently monitored in our Veracode account."

**🤖 AI Agent:**
> I've fetched 3 core tracked applications from your Veracode environment: 
- 'Mobile-Banking-iOS' (GUID: 82a1...)
- 'Legacy-CRM-Core' (GUID: f3b9...)
- 'Auth-Microservice' (GUID: 11c2...)
Would you like me to pull the security finding logs specifically for 'Auth-Microservice'?

---

**👤 You:**
> "Get the detailed security profile for the application GUID 'f3b9...'."

**🤖 AI Agent:**
> Here is the detailed profile for GUID `f3b9-12aa-99bb`: This corresponds to 'Legacy-CRM-Core'. It currently has a 'Very High' Business Criticality rating. Its compliance policy dictates adherence to 'Veracode Recommended High'. However, its recent automated scan status indicates 'Did Not Pass' due to 12 unmitigated critical severity flaws.

---

**👤 You:**
> "Explain finding ID '89' from that app and how to fix it."

**🤖 AI Agent:**
> Finding ID '89' points to an Improper Neutralization of Input (CWE-79), better known as Stored Cross-Site Scripting (XSS). It was found in `user_profile.js` at line 144.

**Description:** Externally supplied, untrusted input is reflected directly into browser DOM executing scripts.

**Remediation:** To fix this, encapsulate the rendered variable `userInput` with a context-savvy encoding library like `DOMPurify` before injecting it via `innerHTML`. 

I can write a quick patch for line 144 if you'd like.


## Installation & Usage

To install and use the **Veracode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veracode](https://vinkius.com/mcp/veracode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
