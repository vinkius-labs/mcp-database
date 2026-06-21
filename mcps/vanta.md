# Vanta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vanta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage your automated compliance and security posture. Audit users, devices, vendors, and vulnerabilities directly from your AI agent.

## Description
Connect your **Vanta** account to any AI agent and bring continuous security monitoring directly into your conversational workflow.

### What you can do

- **Personnel Compliance** — Rapidly list all active personnel records, fetch specific user security training completion details, or deactivate users directly during employee offboarding.
- **Endpoint Fleet** — Retrieve data on all computers and physical workstations actively monitored by Vanta, ensuring disk encryption and antivirus SLA compliance.
- **Vulnerability Tracking** — Monitor unpatched Common Vulnerabilities and Exposures (CVEs) across your cloud infrastructure and verify remediation SLAs in real-time.
- **Security Posture** — Access public Trust Center configurations, review pending security report requests from customers, and list your internal risk-vetted third-party vendors (subprocessors).

### How it works

1. Subscribe to this server
2. Enter your Vanta Developer API Token
3. Start fetching and updating security postures from Claude, Cursor, or any MCP-compatible client

Your AI agent seamlessly becomes an extension of your Security and Compliance operations.

### Who is this for?

- **Security & Compliance Teams** — automate manual compliance evidence-gathering processes through conversational commands instead of hunting through dashboards.
- **IT Administrators** — seamlessly check if new hardware endpoints are properly communicating with Vanta agents.
- **DevSecOps** — query your vulnerability backlog in an instant while planning technical sprints inside an IDE.
- **Sales & GTM Teams** — approve sensitive trust-center whitepaper requests immediately from chatbots.


## Available Tools
- **vanta_compliance_status**: Shows: overall pass rate percentage, number of passing/failing/warning tests per framework, critical alerts requiring immediate attention, and the audit-readiness score. Use when the user asks "how is our compliance?", "are we ready for the SOC 2 audit?", or needs a quick compliance health check across all frameworks.

Get the overall compliance posture dashboard — pass rates per framework, critical alerts, and audit readiness score across SOC 2, ISO 27001, HIPAA, and GDPR
- **vanta_get_test**: Use to drill into a failing test: "why is the MFA test failing?" or "which resources are non-compliant for encryption?"

Get detailed information about a specific Vanta compliance test — evidence, linked controls, failing resources, and remediation guidance
- **vanta_list_computers**: Each device shows: device name, OS version, disk encryption status, firewall enabled, antivirus installed, screen lock configured, owner email, and overall compliance status. Use for endpoint compliance audits, device inventory, or identifying non-compliant machines before an audit.

List monitored endpoint devices — laptops and desktops with OS version, encryption status, antivirus, and compliance state
- **vanta_list_evidence_requests**: Each request includes: description of the evidence needed, assigned owner, due date, completion status, and linked control. Use during audit preparation: "what evidence is still outstanding?", "who needs to submit screenshots?", or "are we ready for the audit?"

List outstanding audit evidence requests in Vanta — documents and screenshots needed from team members with deadlines
- **vanta_list_integrations**: ). Each integration shows: service name, connection status (connected/disconnected/error), last sync date, coverage metrics, and any configuration warnings. Use to check integration health, verify coverage, or troubleshoot sync issues.

List all connected integrations in Vanta — cloud providers, identity providers, code repos, and their sync status
- **vanta_list_people**: Each person includes: name, email, role, security awareness training status (completed/overdue), device compliance (encrypted/antivirus/updated), access review completion, and employment status. Use for "who has overdue training?", "which employees have non-compliant devices?", or pre-audit personnel reporting.

List all personnel in Vanta with security training completion, device compliance, access review status, and onboarding/offboarding state
- **vanta_list_policies**: ). Each policy shows: name, approval status (approved/draft/needs review), last review date, next review due, version number, and percentage of employees who have acknowledged. Use for policy management audits or compliance gap analysis.

List all security and compliance policies in Vanta — approval status, review dates, version tracking, and employee acknowledgment rates
- **vanta_list_risks**: Each risk includes: title, description, risk category, impact level (1-5), likelihood level (1-5), calculated risk score, linked mitigating controls, treatment plan (accept/mitigate/transfer), owner, and status. Use for risk management reporting, board-level summaries, or identifying high-risk areas that need attention.

List the risk register — identified security risks with impact, likelihood, risk score, assigned controls, and mitigation status
- **vanta_list_tests**: Each test maps to a specific control requirement (e.g., "MFA enabled for all users", "Encryption at rest"). Returns test name, associated framework (SOC 2/ISO/HIPAA/GDPR), current status (PASS/FAIL/WARNING), last run date, and any remediation notes. Use when the user asks about compliance posture, failing tests, or audit readiness.

List all compliance monitoring tests in Vanta — SOC 2, ISO 27001, HIPAA, and GDPR controls with pass/fail status and last run dates
- **vanta_list_vulnerabilities**: ). Each entry includes severity (CRITICAL/HIGH/MEDIUM/LOW), CVE identifier, affected resource/package, discovery date, and SLA deadline for remediation. Use when the user asks about security posture, open vulnerabilities, or needs to prioritize remediation work.

List detected security vulnerabilities across your infrastructure — severity, CVE IDs, affected resources, and SLA deadlines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vanta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List pending Trust Center requests for our security documentation."

**🤖 AI Agent:**
> I've retrieved the pending Trust Center requests. You currently have 3 prospects awaiting access: 'sarah@piedpiper.com' requested SOC 2 Type II reports yesterday, and 'admin@hooli.xyz' requested Pen-Test summaries this morning. Would you like me to approve these specific emails for viewing?

---

**👤 You:**
> "Retrieve the Vanta framework compliance details and mapped status of our organization."

**🤖 AI Agent:**
> I retrieved your Vanta organization details. Your company 'Acme Corp' is currently actively tracking towards SOC 2 Type II and HIPAA frameworks. Your continuous monitoring health score sits firmly at 92%. Would you like a breakdown of any failing domains?

---

**👤 You:**
> "What subprocessor vendors are we actively syncing in Vanta right now?"

**🤖 AI Agent:**
> You have 14 active integrations serving as authorized subprocessors logged in Vanta. Major ones include Amazon Web Services, GitHub, Slack, and Datadog. Three minor vendors are currently unverified and missing full justification descriptions in the system policy context.


## ❓ FAQ

**Q: How can I easily check if an employee completed their security training?**
Provide the specific email or ID and ask the agent: `get the Vanta compliance details for John Doe`. The `getUserTool` will retrieve all local profile assertions, confirming immediately whether John completed the security training modules and signed the internal policies.

**Q: Can I automatically view which vulnerabilities span past our SLA threshold?**
Yes. Ask the agent to `list our security vulnerabilities and highlight any that are missing their SLA timelines`. It will fetch the complete collection from Vanta, compute the statuses, and list out the critical unresolved issues requiring immediate developer engineering attention natively.

**Q: What happens when an employee terminates contract? Can I use the agent?**
Absolutely. You can implement instantaneous offboarding by prompting the AI: `deactivate Vanta compliance monitoring for user ID 123456`. The agent utilizes the `updateUserTool` switching their active flags internally to false. Offboarding checklists just got significantly faster.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vanta](https://vinkius.com/mcp/vanta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vanta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vanta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vanta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vanta": {
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
