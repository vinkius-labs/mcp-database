# Serasa ClearSale — Fraud Risk Analysis (Connect & Payment Link) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-clearsale-fraud-risk-analysis-connect-payment-link)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Submit orders and identities for ClearSale fraud scoring, then read the decision, score and insights.

## Description
ClearSale scores transactions for fraud risk across two products, and this connector covers both. Link de Pagamentos analyses an e-commerce order: submit the buyer, the payment and the items, receive an analysisId plus a status code and a 0–100 risk score, then confirm the outcome and feed chargebacks back as calibration. Connect runs an orchestrated analysis through an integration you configure in ClearSale and answers with a decision, coded insights, an optional MFA challenge and a biolink device-binding score. The connector mints its own JWT per product, caches it and refreshes transparently. Responses are rendered as a verdict line — approved, declined or manual review — followed by the score, the insights and the challenge state, so an agent can act without parsing the raw payload.


## Available Tools (7)
- **get_payment_link_order**: The response carries the analysisId, the transactionId you sent, the current status code and the risk score (0–100, higher = riskier). Use it to decide whether to keep waiting, release the order or cancel it.

Read the status, score and result of a ClearSale payment-link analysis
- **mark_chargeback**: ClearSale uses it as negative feedback, which sharpens future scores for the same buyer, card and device signals. code is the order code you submitted; chargeback_date_utc is the acquirer notification date. Send bin or pan plus the card brand when you have them — they strengthen the device/card linkage.

Mark a ClearSale payment-link order as chargeback to calibrate the risk analysis
- **submit_payment_link_order**: ClearSale scores 0–100 where higher is riskier; the status code (e.g. APA for approved, PMA for manual review) tells you what to do next. Poll get_payment_link_order until the status stops changing, then confirm the outcome with update_payment_link_status. The order must identify the buyer (document, name, email), the total value and the payment. Billing is required; shipping defaults to the billing address unless shipping_* fields are given. Use order_data as a full JSON object to set or override any part of the ClearSale payload — it merges over the built body.

Submit an order to the ClearSale Link de Pagamentos API for fraud risk analysis
- **update_payment_link_status**: Send the status you actually applied: PGA when the payment was captured, PGR / a rejection code when you declined, etc. Call it once the decision is final — ClearSale uses it as feedback for future scoring.

Update the status of a ClearSale payment-link order after the risk analysis
- **create_connect_analysis**: The response returns an executionId, an analysisId and a transactionId plus the first decision (status + score), the coded insights, an optional MFA challenge and the biolink verdict. When the MFA status is pending, the flow waits for the user to answer the challenge — poll get_connect_analysis until the decision status is done. integration_id is the id of the integration configured in ClearSale Connect — it selects the flow. payload is the integration request as a JSON object; its fields depend on the integration, so send the document / email / phone / device signals your flow requires.

Run a fraud analysis through a ClearSale Connect integration
- **get_connect_analysis**: The decision status is done once the flow finished; an MFA status of pending means the user has not answered the challenge yet, and biolink reports the device-binding score. The insights array is the coded reasoning behind the decision — each item has a code (e.g. RDR0040), a description, a category, a relevance level and the data points it relates to.

Read the current decision, insights, MFA state and biolink of a ClearSale Connect analysis
- **update_connect_status**: status is a ClearSale code (e.g. APA for approved). Call it once the decision is final so Connect can use the result as feedback.

Update the status of a ClearSale Connect analysis after the decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa ClearSale — Fraud Risk Analysis (Connect & Payment Link)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Score this order: buyer João Silva, CPF 12345678901, email joao@test.com, total BRL 500, paid by PIX, shipped to São Paulo/SP. Widget, BRL 500, qty 1."

**🤖 AI Agent:**
> Calls submit_payment_link_order with the buyer fields, total_value 500, payment_type 27 (PIX), billing_state SP and the item; then polls get_payment_link_order with the returned analysisId until the status settles.

---

**👤 You:**
> "Run the Connect integration INT-7 for document 12345678901 and tell me what the insights say."

**🤖 AI Agent:**
> Calls create_connect_analysis with integration_id INT-7 and payload {"document": "12345678901"}, then get_connect_analysis to read the decision score, the coded insights (e.g. RDR0040) and the MFA / biolink state.

---

**👤 You:**
> "Order ORD-42 from last month was charged back — fraud, BRL 320, Visa. Register it."

**🤖 AI Agent:**
> Calls mark_chargeback with code ORD-42, chargeback_date_utc, dispute_reason 1 (fraude), dispute_value 320, card_brand_id 3 and card_brand VISA so ClearSale uses it as negative feedback.


## ❓ FAQ

**Q: Which product should I use for an e-commerce order?**
submit_payment_link_order — it takes the buyer, the payment and the items and returns a status code plus a 0–100 score. Use Connect (create_connect_analysis) only when you have a configured integration and want its orchestrated flow with insights, MFA and biolink.

**Q: What is a good score?**
ClearSale scores 0–100 where higher means riskier. The status code is the actionable signal: APA is approved, PMA routes to manual review, and rejection codes start with RP. The rendered verdict line maps this for you instead of leaving you to read the raw code.

**Q: Why should I call the status update and chargeback tools?**
They are feedback, not bookkeeping. update_payment_link_status tells ClearSale which decision you actually applied and mark_chargeback reports a later chargeback; both feed the model so future scores for the same buyer, card and device signals get sharper. Skipping them silently degrades the scores you rely on.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-clearsale-fraud-risk-analysis-connect-payment-link](https://vinkius.com/en/ai-agent-connect/serasa-clearsale-fraud-risk-analysis-connect-payment-link)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa ClearSale — Fraud Risk Analysis (Connect & Payment Link)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-clearsale-fraud-risk-analysis-connect-payment-link` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa ClearSale — Fraud Risk Analysis (Connect & Payment Link)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-clearsale-fraud-risk-analysis-connect-payment-link": {
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
