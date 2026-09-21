# Serasa Experian Credit Monitoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-experian-credit-monitoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Let AI agents watch CPFs and CNPJs for credit events — build monitoring rules, add documents, read alerts, and wire up webhooks.

## Description
Connect your **Serasa Experian** account so any AI agent can run the full credit-monitoring lifecycle — using Serasa's official Monitoring API.

### What you can do

- **Discover what to watch** — the subject catalog lists every attribute a rule can monitor: negative annotations (pefin/refin, SPC), notary records, judgement filings, bankruptcy and shareholding participation, plus score families (HAT3, H4PJ, HPJM, H5RC, H5RA) with their allowed custom interval ranges
- **Create and manage rules** — a rule binds a name, a document type (CPF/CNPJ), the variable ids and the alert emails; pause or reactivate without deleting
- **Manage the monitored portfolio** — add or remove up to 1000 documents per batch and list every monitored document with its rules, inclusion dates and status
- **Read and triage alerts** — alerts fire when a watched attribute changes; filter by document, rule name or read status, aggregate per document for portfolio triage, and mark them read
- **Follow operational notifications** — system events for rule creation, document processing and exclusions, distinct from credit alerts
- **Push instead of poll** — register webhooks (an AUTH endpoint plus one or more subject endpoints) and Serasa pushes the alerts to your system

### How it works

The server authenticates with your Client ID / Client Secret, caches the Bearer token and re-authenticates transparently on expiry. Filters are rendered in the API's deep-object format automatically — pass plain values, not query strings.


## Available Tools (14)
- **add_monitored_documents**: `documents` is a JSON array or a comma list; non-digits are stripped. The response separates accepted from rejected documents with per-document error codes (e.g. MDC412 — already monitored). A 207 response means partial success and is still returned as a result, not an error.

Add CPFs or CNPJs to an existing monitoring rule
- **create_monitoring_rule**: Returns the rule `id`, which you pass to add_monitored_documents. `variables` is a JSON array of numeric ids or a comma list like "1,2,3". Score variables accept optional interval overrides via variables_config (JSON array of {"id","intervalMode":"CUSTOM","minValue","maxValue"}). To watch partners/shareholders, set rule type to CNPJ and pass partner variable ids in partners_variables.

Create a monitoring rule that watches credit events for a list of CPFs or CNPJs
- **delete_webhook**: Poll list_alerts afterwards to keep read visibility of the events.

Delete a webhook by id, stopping alert delivery to its endpoints
- **list_alerts**: Filter by document number (comma list accepted), viewed/deleted status, document type or the rule name. `unlink_document=true` includes alerts for documents already removed from monitoring. Use summarize_alerts for counts and mark_alerts_read to clear the queue.

List credit-event alerts generated for the monitored documents
- **list_monitored_documents**: Filter by document number, rule id or active status; date filters (included_at_start/included_at_end) are ISO 8601. The summary block reports how many monitoring links still have a future expiration date and the product types in play.

List the documents currently monitored, with their rules, inclusion dates and status
- **list_monitoring_rules**: Use the rule id with add_monitored_documents / remove_monitored_documents, and filter alerts by the rule name. Set active=false to list only inactive rules.

List the monitoring rules already created in the organization
- **list_monitoring_subjects**: Each subject exposes `variables` — the numeric ids you pass to create_monitoring_rule. Call this first to discover the variable ids for the document type you monitor. Score subjects also show the allowed custom interval range (valueMin–valueMax).

List the monitoring subjects (attributes/variables) available for CPF, CNPJ or partners
- **list_notifications**: Filter by subtype, type (INFO/WARNING/ERROR) or read status; created_at takes one or two ISO dates that form a range.

List operational notifications about the monitoring itself — rule creation/activation, document processing and exclusions
- **list_webhooks**: Use the id with delete_webhook.

List the registered webhook endpoints for alert delivery
- **mark_alerts_read**: Clearing the queue keeps list_alerts results available with viewed=true.

Mark one or more alerts as read so they leave the unread queue
- **register_webhook**: Pass them as a JSON array of {"type","endpoint"} objects. The credentials (clientId/clientSecret) authenticate the delivery, not this call.

Register webhook endpoints so Serasa pushes alerts to your system instead of only polling
- **remove_monitored_documents**: Documents removed here stop generating alerts for this rule but keep their alert history. The response mirrors the add format (accepted/rejected lists).

Remove CPFs or CNPJs from a monitoring rule
- **summarize_alerts**: Pairs well with a document_number filter for a single customer.

Aggregate alerts by document — total counts and unread counts per monitored CPF/CNPJ
- **update_monitoring_rule**: Omitted optional fields keep their current value on the Serasa side only when not sent. Pass active=false to pause a rule without deleting it — its documents stop being monitored. Rule id comes from list_monitoring_rules.

Update a monitoring rule: rename it, change the watched variables, alert emails or active status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa Experian Credit Monitoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Set up monitoring for CNPJ 33.014.556/0001-96: watch for negative annotations and bankruptcy, sending alerts to risk@company.com."

**🤖 AI Agent:**
> I created the rule "Negatives & Bankruptcy" (id 42, type CNPJ) with the variables for negative annotations and bankruptcy, and added the CNPJ to it. The document is now monitored; alerts will be sent to risk@company.com.

---

**👤 You:**
> "What happened with the monitored portfolio this week? Just give me the highlights."

**🤖 AI Agent:**
> I aggregated the alerts per document. 5 of the 120 monitored documents had events this week: 3 new negative annotations, 1 notary record, and 1 score drop below the configured interval. The most affected is CNPJ 12.345.678/0001-90 with 2 events, both unread.

---

**👤 You:**
> "Register a webhook so alerts get pushed to our collector at https://collector.example.com/serasa."

**🤖 AI Agent:**
> I registered the webhook (id 7): the AUTH endpoint at https://collector.example.com/serasa/auth validates delivery, and ATTRIBUTE_NEGATIVE points to https://collector.example.com/serasa/negative. Serasa will now push negative-annotation alerts there instead of only being pollable.


## ❓ FAQ

**Q: What is the difference between an alert and a notification?**
An **alert** is a credit event on a monitored document — a new negative annotation, a notary record, a bankruptcy filing, or a score crossing the configured interval. A **notification** is an operational event about the monitoring itself: rule created or activated, document batch processed, documents excluded, report downloaded. Alerts are the business signal; notifications are the audit trail.

**Q: How do I know which variable ids to put in a rule?**
Call `list_monitoring_subjects` first — it returns each subject (Negative, SpcNegative, Bankruptcy, NotaryRecord, HAT3, …) with its numeric id, the document types it applies to, and, for score subjects, the allowed custom interval range. The `variables` you pass to `create_monitoring_rule` are exactly those ids, as a JSON array or a comma list like "1,2,3".

**Q: Why did adding documents return a 207 with some rejections?**
A 207 means the batch was partially accepted: some documents went through, others were rejected. The result separates them into accepted and rejected lists with per-document error codes — the most common is a document already monitored by that rule. Only genuinely invalid input or an auth failure fails the whole call.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-experian-credit-monitoring](https://vinkius.com/en/ai-agent-connect/serasa-experian-credit-monitoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa Experian Credit Monitoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-experian-credit-monitoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa Experian Credit Monitoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-experian-credit-monitoring": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
