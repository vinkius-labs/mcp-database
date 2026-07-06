# Drata MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Automate compliance and security via Drata — monitor controls, track personnel onboarding, audit policies, and verify cloud asset security directly from any AI agent.

## Description
Connect your **Drata** account to any AI agent and take full control of your continuous compliance and automated security monitoring through natural conversation.

### What you can do

- **Compliance Control Oversight** — List internal compliance controls and fetch exact evaluation states to see if technical or administrative requirements are passing or failing
- **Personnel Compliance Tracking** — Monitor employee and contractor directories to identify missing security training, background checks, or policy acknowledgments
- **Security Policy Auditing** — Retrieve the overarching InfoSec documentation and extract renewal dates and completion rates to assess audit readiness
- **Automated Test Monitoring** — Detail which technical monitors across AWS, GCP, or Azure are triggering compliance deviations in real-time
- **Framework Readiness** — Track active compliance frameworks (SOC 2, ISO 27001, HIPAA) and get overall readiness scores and control completion percentages
- **Vendor Risk Management** — Returns the vendor risk inventory to track security questionnaires and data risk classifications for third-party subprocessors
- **Cloud Asset Verification** — Insight into how EC2, RDS, and other infrastructure nodes align against underlying compliance controls

### How it works

1. Subscribe to this server
2. Enter your Drata Public API Key (found in your Drata Dashboard under Settings > API Keys)
3. Start managing your compliance workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Compliance Officers & CISOs** — audit control statuses and policy readiness without manual dashboard navigation
- **HR & Ops Teams** — monitor personnel onboarding milestones and background check clearances using natural language
- **Security Engineers** — verify cloud asset alignment and monitor automated test failures in real-time
- **Developers** — test and debug continuous compliance integrations through natural conversation


## Available Tools (10)
- **drata_list_assets**: Each asset shows: resource type, resource ID, compliance status against linked controls, encryption-at-rest verification, network boundary adherence, and associated region/VPC. Use when the user asks about infrastructure compliance, unencrypted resources, or needs an asset inventory for audit evidence.

List cloud infrastructure assets monitored by Drata — EC2 instances, RDS databases, S3 buckets, and other resources with compliance status
- **drata_list_controls**: Each control represents a specific requirement (e.g., "Passwords must be 12+ characters", "MFA enabled for all users", "Encryption at rest required"). Returns control name, description, passing/failing status, mapped framework(s), linked tests, and control owner. Use when the user asks about compliance posture, failing controls, or audit gap analysis.

List all compliance controls in Drata — the discrete technical and administrative requirements mapped to SOC 2, ISO 27001, HIPAA, and GDPR frameworks
- **drata_list_frameworks**: Each framework shows: name, version, overall readiness score, percentage of controls passing, number of controls mapped, and target audit date. Provides a high-level view of multi-framework compliance posture. Use for board-level reporting, audit planning, or determining which framework needs the most attention.

List active compliance frameworks tracked by the Drata workspace — SOC 2 Type II, ISO 27001, HIPAA, GDPR, PCI DSS — with readiness scores
- **drata_list_personnel**: Each person includes: name, email, role, employment type, Security Awareness Training status (completed/overdue/not started), device compliance (MDM enrolled, encrypted, antivirus), background check clearance, and policy acceptance rates. Use for "who is non-compliant?", "which employees have overdue training?", or pre-audit personnel reporting.

List all tracked personnel in Drata with security training status, device compliance, background check clearance, and policy acceptance
- **drata_list_policies**: Each policy includes: name, category, CISO approval status, version number, last review date, next review due, and employee acknowledgment completion rate. Policies are mandatory for SOC 2 / ISO 27001. Use when the user asks about policy status, which policies need review, or audit readiness regarding documentation.

List all security and compliance policies in Drata — Information Security, Data Classification, Incident Response, Acceptable Use, and more
- **drata_list_tests**: Each test monitors a specific technical requirement in real-time (e.g., "S3 Buckets must not be public", "GitHub branch protection enabled", "MFA enforced in Okta"). Shows test name, associated control, pass/fail status, last evaluation time, and failing resources if any. Use when the user asks about automated monitoring, which checks are failing, or real-time compliance status.

List Drata automated continuous compliance tests — real-time monitors checking AWS, GitHub, Okta, and other integrations for security deviations
- **drata_list_vendors**: Each vendor includes: company name, data risk classification (Critical/High/Medium/Low), security questionnaire completion status, SOC 2 report review status, last assessment date, data categories shared, and assigned risk owner. Use for vendor risk assessment, subprocessor audits, or evaluating the security posture of your supply chain.

List third-party vendors in Drata vendor risk management — risk classification, security questionnaire status, and SOC 2 report reviews
- **drata_get_control**: Returns passing/failing status, which automated tests provide evidence for this control, the explicit auditor language defining the risk logic, and any manual evidence uploads. Use to investigate why a control is failing, what evidence supports it, or to prepare for auditor questions about a specific requirement.

Get detailed status of a specific Drata control — pass/fail state, automated test evidence, and auditor-facing risk language
- **drata_get_person**: Returns MDM (Jamf/Intune) enrollment status, background check clearance date, onboarding milestone completion, linked IdP (Okta/Google Workspace) groups for access control mapping, security training completion date, and any compliance gaps. Use when investigating a specific employee compliance issue.

Get the compliance onboarding state of a specific employee — MDM enrollment, background checks, IdP grouping, and training milestones
- **drata_get_policy**: Essential for assessing audit readiness regarding mandatory annual document refreshes.

Get detailed status of a specific Drata policy — renewal dates, employee acknowledgment rates, owner assignment, and version history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drata** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all failing compliance controls"

**🤖 AI Agent:**
> Retrieving control statuses... I found 3 failing controls: 'MFA for IdP Users', 'Encrypted Backups', and 'Vulnerability Scanning'. Would you like to see the automated test results for any of these?

---

**👤 You:**
> "What is the compliance onboarding status for employee John Doe?"

**🤖 AI Agent:**
> John Doe's status: Background check cleared, Security training completed, but 'Acceptable Use Policy' is still pending acknowledgment. I can send him a reminder if you'd like.

---

**👤 You:**
> "List my active compliance frameworks and readiness scores"

**🤖 AI Agent:**
> You have 2 active frameworks: SOC 2 Type II (85% Ready) and ISO 27001 (72% Ready). I can provide a breakdown of the remaining controls for either framework.


## ❓ FAQ

**Q: Can my agent check if specific employees have finished their security training?**
Yes. Use the 'list_personnel' or 'get_personnel_status' tools. The agent retrieves the onboarding state, including Security Awareness Training completion and background check clearance for any tracked individual.

**Q: How do I monitor which compliance controls are currently failing?**
Use the 'list_controls' tool to see all controls and 'get_control' for specific details. The agent will fetch exact evaluation states and automated test results to identify failing requirements and their risk logic.

**Q: Can I see my SOC 2 readiness score through natural conversation?**
Absolutely. Use the 'list_frameworks' tool. Your agent will pull the top-level standard boundaries and provide overall readiness scores and aggregated control completion percentages for frameworks like SOC 2.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drata](https://vinkius.com/mcp/drata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drata** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drata** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drata": {
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
