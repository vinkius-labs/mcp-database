# Serasa Experian PowerCurve — Credit Decision Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-experian-powercurve-credit-decision-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Submit credit proposals to PowerCurve and read back the decision, score and policy outcome.

## Description
Serasa Experian PowerCurve is the decision engine that scores a credit proposal against the lender's own policy and returns an approve / decline / refer verdict together with the enrichment blocks the decision was based on. This connector covers the screenless (headless) application API: submit a proposal for the standard, Fintech and Coad flows, query the status of an existing application, and reprocess one. The connector mints its own JWT from the username / password pair, caches it for its lifetime and refreshes transparently. Responses are rendered as the verdict, the scores and ratings, the Serasa enrichment and the applicant summary, so an agent can reason about the outcome without reading the raw DV-* blocks.


## Available Tools (5)
- **get_proposal_status**: Use it to poll proposals submitted asynchronously, or to resync after a timeout. The response carries the same decision blocks as the submit calls.

Look up proposals and refresh their processing status from PowerCurve
- **reprocess_proposal**: Useful when the underlying Serasa data changed, a policy was updated, or the first run returned a refer decision you want re-evaluated with corrected input. Identify the target by application_id or numero_proposta.

Re-run the decision flow on an existing PowerCurve proposal, e.g. after data changes
- **submit_coad_proposal**: Its request body uses the Coad input definition, so send the Coad-specific fields via extra_data and use the typed parameters for the parts the two flows share.
`numero_proposta` is your own proposal identifier; `id_servico` selects the service configured in PowerCurve. The product block (produto, valor_emprestimo / valor_credito, prazo, finalidade, subprodutos) describes what the customer is asking for. The applicant block carries the person's identity. Anything the typed parameters do not cover can be sent as a full `extra_data` JSON object, which is merged over the built body.

Submit a proposal through the Coad flow for co-advised or consortium credit
- **submit_fintech_proposal**: Use it when your contract with Serasa is the Fintech service rather than the generic NovaProposta one.
`numero_proposta` is your own proposal identifier; `id_servico` selects the service configured in PowerCurve. The product block (produto, valor_emprestimo / valor_credito, prazo, finalidade, subprodutos) describes what the customer is asking for. The applicant block carries the person's identity. Anything the typed parameters do not cover can be sent as a full `extra_data` JSON object, which is merged over the built body.

Submit a proposal through the Fintech flow, optimised for real-time digital onboarding
- **submit_proposal**: The response also carries the enriched Serasa data the decision was based on (score, restrictions, income range, risk level), so one call is often the whole underwriting step.
`numero_proposta` is your own proposal identifier; `id_servico` selects the service configured in PowerCurve. The product block (produto, valor_emprestimo / valor_credito, prazo, finalidade, subprodutos) describes what the customer is asking for. The applicant block carries the person's identity. Anything the typed parameters do not cover can be sent as a full `extra_data` JSON object, which is merged over the built body.

Submit a credit proposal to PowerCurve and get the automated decision (approve, deny or refer)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa Experian PowerCurve — Credit Decision Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decide this loan request: proposal P-1024, service SVC-EMP, applicant João Silva, CPF 12345678901, born 1985-03-10, requesting BRL 5000 over 12 months."

**🤖 AI Agent:**
> Calls submit_proposal with numero_proposta P-1024, id_servico SVC-EMP, primeiro_nome João, sobrenome Silva, cpf 12345678901, data_nascimento 1985-03-10, valor_emprestimo 5000, prazo 12. Returns the verdict (approve / decline / refer), the score, the Serasa enrichment and the application id.

---

**👤 You:**
> "Check where application APP-7731 stands and re-run the decision if it is stale."

**🤖 AI Agent:**
> Calls get_proposal_status with application_id APP-7731 to read the current status and decision, then reprocess_proposal with the same application_id to re-run the flow.

---

**👤 You:**
> "Submit this to the Fintech flow and also capture the Bacen database the policy consumed."

**🤖 AI Agent:**
> Calls submit_fintech_proposal with the proposal fields plus extra_data {"DV-Bacen": {"Bacen": [{"Database": "DB1"}]}} so the custom block is merged over the built body.


## ❓ FAQ

**Q: Which flow should I submit a proposal to?**
submit_proposal is the standard screenless flow. submit_fintech_proposal is the Fintech variant and submit_coad_proposal adds the Coad-specific blocks. If you do not know which one applies, start with submit_proposal and check the returned service id with the provider of the flow.

**Q: Why are optional applicant fields sometimes ignored?**
Each flow accepts a subset of the applicant and request fields. The connector only puts a field in the body when the flow's schema declares it, so sending produto or prazo to a flow that does not use them is a no-op rather than an error. Use extra_data to set any other DV-* block exactly as PowerCurve expects it.

**Q: What does a refer verdict mean?**
The policy could not approve or decline automatically — a human analyst must review the case. The rendered output keeps the decision name, the recommendation codes and the Serasa enrichment so the analyst has the reasons in one place. Call reprocess_proposal after the review to re-run the decision.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-experian-powercurve-credit-decision-engine](https://vinkius.com/en/ai-agent-connect/serasa-experian-powercurve-credit-decision-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa Experian PowerCurve — Credit Decision Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-experian-powercurve-credit-decision-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa Experian PowerCurve — Credit Decision Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-experian-powercurve-credit-decision-engine": {
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
