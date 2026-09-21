# Serasa Infomais — People & Organization Enrichment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-infomais-people-organization-enrichment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Enrich CPFs and CNPJs with dozens of attributes, and reverse-lookup documents from partial data.

## Description
Infomais is Serasa Experian's data-enrichment service (MS Data Delivery). Request exactly the attributes you need for a CPF or CNPJ and pay only for those. People attributes cover identity (name, birth date, mother's name, RG), contacts (addresses, phones, e-mails), profiling (income, social class, mosaic, purchasing power, scholarity), marketing affinities (credit card, personal credit, e-commerce, travel, smartphone, investments) and compliance (PEP, NIS, Bolsa Família, federal employee). Organization attributes cover registration (business and fantasy names, opening date, legal nature, CNAE, status), contacts, sizing (presumed revenue, company size, employee range, social capital, Simples Nacional), governance (partners, legal representative, board, social composition) and compliance (Sintegra, CCM, Suframa, cadastral situation).

Two reverse-lookup endpoints find a document from partial data — a name plus a city, a phone, an address — for people and organizations, and a lighter filter endpoint identifies records by name, UF and date. The distributor variant is supported through the distributor_type and distributor_dw parameters. Authentication is OAuth2 client credentials issued at developer.serasaexperian.com.br; the reverse-lookup endpoints also require a user token.


## Available Tools (5)
- **enrich_organization**: `attributes` is a JSON array or a comma list; only the names the organization endpoint supports are accepted, so a typo is reported rather than silently ignored. The response mirrors the requested attributes — request exactly what you need, since each attribute is a billable item.

Useful combinations: ["businessName","fantasyName","openingDate","legalNature","cnae","registrationStatus"] for registration; ["addresses","phones","email"] for contacts; ["presumedRevenue","companySize","employeeRange","socialCapital","simplesNacional"] for sizing; ["businessPartners","legalRepresentative","boardAdministrator","socialComposition"] for governance; ["sintegra","ccm","suframa","cadastralSituation","operationalIndicator"] for compliance; ["matrizFilial","branchsCount","codIBGE"] for structure.

`indirect_sale_document` is accepted only on the distributor variant.

Enrich a CNPJ with the requested Infomais attributes: registration, partners, revenue and more
- **enrich_person**: `attributes` is a JSON array or a comma list; only the names the person endpoint supports are accepted, so a typo is reported rather than silently ignored. The response mirrors the requested attributes — request exactly what you need, since each attribute is a billable item.

Useful combinations: ["name","birthDate","motherName","gender","maritalStatus","rg"] for identity; ["addresses","phones","email","emailValidado"] for contacts; ["income","socialClass","mosaic","purchasingPower","scholarity","profession"] for profiling; ["afinidadeCartaoCredito","afinidadeCreditoPessoal","afinidadeEcommerce",...] for marketing affinities; ["pep","nis","bolsaFamilia","federalGovEmployee"] for compliance checks.

`distributor_type` and `distributor_dw` apply only to the distributor variant of the product; leave them unset otherwise.

Enrich a CPF with the requested Infomais attributes: name, contacts, income, affinities and more
- **filter_enrichment**: Infomais answers with the document it resolved plus name, age, city, neighborhood and uf — use it to validate a document before calling enrich_person or enrich_organization. This endpoint also requires a user token: set `user_token`.

Resolve loose data about a person or organization to candidate documents
- **find_organization_by_keys**: The endpoint is `enrichments/organizations/retrieve` and it requires a user token in addition to the client token — set `user_token` to the USER token issued for your application. `response_limit` caps the number of candidates.

Find CNPJs matching partial data — corporate name, CEP, phone — without knowing the document
- **find_person_by_keys**: The endpoint is `enrichments/person/retrieve` and it requires a user token in addition to the client token — set `user_token` to the USER token issued for your application. `response_limit` caps the number of candidates.

Find CPFs matching partial data — name, address, phone, birth date — without knowing the document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa Infomais — People & Organization Enrichment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich this lead: CPF 12345678901. I need name, contacts and marketing affinities."

**🤖 AI Agent:**
> Calls enrich_person with document 12345678901 and attributes ["name","birthDate","addresses","phones","email","afinidadeCartaoCredito","afinidadeEcommerce","socialClass","mosaic"], returning only the requested attributes.

---

**👤 You:**
> "I have a company name and a city but no CNPJ — can you find it?"

**🤖 AI Agent:**
> Calls find_organization_by_keys with corporate_name and city plus your user_token, returning candidate organizations with their documents so you can then enrich the right CNPJ.

---

**👤 You:**
> "Check the registration status and partners of CNPJ 33014556000196."

**🤖 AI Agent:**
> Calls enrich_organization with document 33014556000196 and attributes ["businessName","registrationStatus","cadastralSituation","businessPartners","legalRepresentative"].


## ❓ FAQ

**Q: Which attributes should I request?**
Only the ones you will use — Infomais bills per requested attribute. The connector rejects attribute names the endpoint does not support, so a typo fails loudly instead of returning a partial record you pay for without noticing.

**Q: What is the user_token for?**
The reverse-lookup endpoints (find_person_by_keys, find_organization_by_keys and filter_enrichment) require a user token in addition to the client token. Generate it in the same developer portal and pass it per call; the connector forwards it to the right header automatically.

**Q: How do the distributor parameters work?**
They apply only to the distributor variant of Infomais. distributor_type selects the model (NONE, DH, OF or DW) and distributor_dw switches between Distributor DW and Distributor OF. enrich_organization also accepts indirect_sale_document for indirect sales. Leave them unset when your contract is the standard one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-infomais-people-organization-enrichment](https://vinkius.com/en/ai-agent-connect/serasa-infomais-people-organization-enrichment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa Infomais — People & Organization Enrichment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-infomais-people-organization-enrichment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa Infomais — People & Organization Enrichment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-infomais-people-organization-enrichment": {
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
