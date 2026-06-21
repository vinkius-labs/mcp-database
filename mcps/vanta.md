# Vanta MCP Server

Manage your automated compliance and security posture. Audit users, devices, vendors, and vulnerabilities directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vanta)

## Overview
**Category:** fort-knox
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Vanta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vanta](https://vinkius.com/mcp/vanta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
