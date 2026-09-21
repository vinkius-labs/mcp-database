# Serasa Verify ID — Identity Verification & Enrichment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-verify-id-identity-verification-enrichment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify people and companies against the Serasa base, enrich registrations and request fraud scores.

## Description
Verify ID is Serasa Experian's identity-verification and enrichment product. Submit the registration data you collected for a person or a company and receive a coded validation result per attribute, a verification score and a risk verdict. This connector exposes the synchronous verification endpoints for PF and PJ, the batch verification for a list of people, the enrichment endpoints that return the registration data Serasa holds plus the contracted fraud scores, and the PEP file listing. Enrichment answers asynchronously for some packages; the connector returns the requestId and reads the result back on demand. Closed sets such as score_parameters, packages and scores are validated before the call so an invalid value is caught locally instead of consuming a paid request. Authentication is OAuth2 client credentials issued at developer.serasaexperian.com.br.


## Available Tools (8)
- **enrich_organization**: The reply can be asynchronous — when it carries a requestId, poll get_organization_enrichment.

Enrich a company with registration data from Verify ID
- **enrich_person**: package is the data you want back (BASIC, ONLINE_ASYNC, PEP, phone, presumedIncome, profession, PLUS_1, SCHOLARITY, PLD_FLAG, PLD, SEGMENT, REGISTRATIONSTATUS, PVE, PVE_FLAG, ALERTS, FAROL_APOSTADOR, NATIONALITY, PRESUMEDINCOME_2); score is the risk scores you want computed (FRAUD_SCORE_PF, ALERTA_LARANJA_PF, SCORE_C_CADASTRO, TRANSACIONAL, AUTO_FRAUDE, EMAIL, SCORE_C_CADASTRO_CUSTOM_1, ALERTA_LARANJA_PF_2, SCORE_C_CADASTRO_CUSTOM_2, ALERTA_LARANJA_PF_VALOR_1, SCORE_POSITIVO, FRAUDE_VEICULOS, SCORE_CUSTOM_P1, SCORE_CUSTOM_P2, SCORE_CUSTOM_B2, SCORE_CUSTOM_C1, SCORE_CUSTOM_C2, ALERTA_LARANJA_PF_4). The reply is asynchronous for some packages — when the response carries a requestId instead of the data, poll get_person_enrichment until it is done.

Enrich a person with registration packages and request fraud scores from Verify ID
- **get_organization_enrichment**: Poll this until the response carries the data instead of the pending marker.

Read back the result of an asynchronous company enrichment by its requestId
- **get_person_enrichment**: Poll this until the response carries the data instead of the pending marker.

Read back the result of an asynchronous person enrichment by its requestId
- **list_pep_files**: Use it to see which PEP snapshots are available before consulting them through the PEP endpoints.

List the PEP (politically exposed person) files available to this client
- **verify_organization**: Send the CNPJ plus the registration data you collected; score_parameters accepts VERIFY, VERIFY_DISTINCT and REQUEST (FRAUD is person-only). The response shape is the same: coded attribute results, verificationScore and verificationRisk.

Verify a company's registration data against the Serasa base and get a verification score
- **verify_people_batch**: people is a JSON array of objects, each with its own id plus the attributes to verify (document, name, birthDate, motherName, email, phone, address). The response is an array with one verification result per person, in the same order. Prefer this over looping verify_person when you have a whole list to check.

Verify several people's registration data in one synchronous batch call
- **verify_person**: g. "Risco baixo"). Send every attribute you have — the more attributes, the more precise the score. score_parameters controls what the score counts: VERIFY, VERIFY_DISTINCT, REQUEST, FRAUD. Use verify_organization for a CNPJ.

Verify a person's registration data against the Serasa base and get a verification score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa Verify ID — Identity Verification & Enrichment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the registration data for CPF 12345678901: name Joao Silva, born 1985-03-12, email joao@example.com."

**🤖 AI Agent:**
> Calls verify_person with the document, name, birth_date and email, then returns the per-attribute validation results, the verificationScore and the verificationRisk verdict.

---

**👤 You:**
> "Check a whole list of customers at once."

**🤖 AI Agent:**
> Calls verify_people_batch with a JSON array of people, each carrying its own id and attributes, and returns one verification result per person in the same order.

---

**👤 You:**
> "Enrich CPF 12345678901 with the basic registration package and a fraud score."

**🤖 AI Agent:**
> Calls enrich_person with packages BASIC and scores FRAUD_SCORE_PF. If the answer carries a requestId, it polls get_person_enrichment until the data arrives.


## ❓ FAQ

**Q: What is the difference between verification and enrichment?**
Verification compares the data you send against the Serasa base and answers per attribute whether it matches, using verify_person / verify_organization / verify_people_batch. Enrichment returns the registration data Serasa actually holds for that document, plus the fraud scores you request, using enrich_person / enrich_organization.

**Q: What do verificationScore and verificationRisk mean?**
verificationScore is the numeric score produced for that verification and verificationRisk is the verdict Serasa attaches to it, such as Risco baixo, Risco moderado or Risco alto. The distinct flag marks whether the registration data diverges from the data you informed.

**Q: The enrichment came back with a requestId instead of the data — what now?**
Some packages are processed asynchronously. Poll get_person_enrichment or get_organization_enrichment with that requestId until the response carries the data instead of the pending marker.

**Q: Which score parameters can I use?**
Person verification accepts VERIFY, VERIFY_DISTINCT, REQUEST and FRAUD; company verification accepts VERIFY, VERIFY_DISTINCT and REQUEST. Enrichment packages and scores are separate lists documented on each tool — the connector rejects anything outside them before calling the API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-verify-id-identity-verification-enrichment](https://vinkius.com/en/ai-agent-connect/serasa-verify-id-identity-verification-enrichment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa Verify ID — Identity Verification & Enrichment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-verify-id-identity-verification-enrichment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa Verify ID — Identity Verification & Enrichment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-verify-id-identity-verification-enrichment": {
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
