# Pennylane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pennylane)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage French accounting workflows via Pennylane — track invoices, customers, suppliers, and synchronize estimates dynamically using AI.

## Description
Equip intelligent LLM instances with robust access traversing the **Pennylane Accounting API**. Programmatically instantiate global CRM states (customers/suppliers), evaluate bounded sales configurations mapping formal invoices, cross-check estimates gracefully, and execute catalog updates explicitly within structural French accounting compliance.

### What you can do

- **Client & Vendor Management** — Discover active network bounds testing logic reading registered structures handling explicit CRM instances securely
- **Invoice Abstraction** — Execute pure checks isolating boundaries that load explicit arrays of emitted estimates, vendor invoices, or direct accounts receivable operations
- **Catalog Maintenance** — Generate creation boundaries passing formal structures natively instantiating `create_product` logic seamlessly globally
- **Financial Topology** — List accounting category structures tracing pure parameters driving correct semantic allocations natively

### How it works

1. Logically bind the integration instance natively inside Vinkius
2. Introduce your explicit Pennylane Bearer API Token securely mapped below
3. Evaluate dynamic arrays validating global invoicing natively using semantic texts 

### Who is this for?

- **French Accounting Teams** — cross-check specific array records checking missing vendor receipt inputs tracking formal financial metrics directly avoiding visual dashboards
- **B2B Sales Admins** — pull dynamic `estimates` validating accepted loops automatically pushing constraints without friction explicitly
- **ERP Integrations** — use natural logic bounds testing strict invoice lists matching parameters reliably across distributed platforms


## Available Tools
- **list_customers**: Lister tous les clients enregistrés dans Pennylane
- **get_customer_details**: Consulter les détails complets d'un client
- **create_customer**: Créer un nouveau client dans Pennylane
- **list_suppliers**: Lister tous les fournisseurs
- **get_supplier_details**: Consulter les détails d'un fournisseur
- **list_customer_invoices**: Lister toutes les factures clients émises
- **get_customer_invoice_details**: Consulter les détails d'une facture client (lignes, TVA, montants HT/TTC)
- **list_supplier_invoices**: Lister toutes les factures fournisseurs (achats)
- **list_estimates**: Lister tous les devis émis
- **get_estimate_details**: Consulter les détails d'un devis (lignes, TVA, validité)
- **list_products**: Lister tous les produits et services du catalogue
- **create_product**: Créer un nouveau produit ou service dans le catalogue comptable
- **list_categories**: Lister les catégories comptables (plan comptable)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pennylane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trace explicitly the active vendor/supplier lists returning limits logically fetched from the target server."

**🤖 AI Agent:**
> Mapped parameters resolving native arrays. Logged 12 explicit supplier boundaries efficiently checking instances. Top supplier returned natively is 'Azure Subscriptions' mapping ID 55x. Proceed tracking JSON internal limits for ID 55x?

---

**👤 You:**
> "Execute checking bounds strictly creating a new native CRM product called 'Design Consulting' logically priced at 120.00 EUR (VAT 20)."

**🤖 AI Agent:**
> Dispatched JSON gracefully processing boundaries globally over Pennylane REST loops natively tracking. Limits established assigning Product ID strictly 'prd_89a' evaluating parameters completely natively successfully matching target specifications.

---

**👤 You:**
> "Read explicit parameter loops parsing detailed lines bounding Invoice ID 'inv_1092'."

**🤖 AI Agent:**
> Boundaries evaluated tracking `get_customer_invoice_details`. Total target explicitly checks 240.00 EUR natively mapped gracefully tracking 2 explicit lines strictly identifying bounds. Would you like a JSON tabular output gracefully extracting line limits?


## ❓ FAQ

**Q: Can I natively issue payments automatically through bounding API calls on Invoices?**
Explicit boundaries mapped here focus solely on abstract tracking limits parsing creation/retrieval properties. Executing hard external payouts asynchronously requires separate decoupled limits and is prohibited deliberately for financial safety.

**Q: How do estimates structural data distinguish explicit targets returning statuses?**
Yes. Upon passing explicit bounds invoking `list_estimates`, the JSON array returns specific limits resolving internal document parameters perfectly natively—including accepted, invoiced, or natively refused semantic values natively attached.

**Q: Where strictly do I generate and manage this API key securely mapping bounds?**
Navigate standard arrays visually tracing your native Pennylane setup, isolate the explicitly defined 'Parameters > API' log routing explicitly, generating a long-lived generic Bearer structurally starting with `pl_`. Insert gracefully below.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pennylane](https://vinkius.com/mcp/pennylane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pennylane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pennylane` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pennylane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pennylane": {
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
