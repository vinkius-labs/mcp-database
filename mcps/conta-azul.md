# Conta Azul MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conta-azul)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage Brazilian ERP via Conta Azul — track customers, products, services, sales, and monitor financial contracts directly from any AI agent.

## Description
Connect your **Conta Azul** account to any AI agent and take full control of your Brazilian business ERP and financial management through natural conversation.

### What you can do

- **Customer Management** — List and search for customers (PJ/PF), audit fiscal documents (CNPJ/CPF), and create new financial entities natively
- **Inventory & Services** — Map physical products (SKU) and intangible services, retrieve pricing, units of measure, and create new billable components
- **Sales Monitoring** — List continuous logs of confirmed sales, retrieve detailed accounting matrices for units, and verify invoice statuses
- **Recurrence Tracking** — Audit financial contracts and automatic agreements to monitor monthly/annual technical debt and expiration dates
- **Fiscal Compliance (NF-e)** — Retrieve governmental emissions records (NF-e) and validate SEFAZ approval statuses for product invoices
- **Financial Structure** — Access hierarchical category trees (DRE) and map bank accounts to reconcile monetary positions and internal cash flow

### How it works

1. Subscribe to this server
2. Enter your Conta Azul OAuth 2.0 Access Token (found in the Developer Portal under your Application)
3. Start managing your Brazilian ERP from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners (Brazil)** — monitor sales volume and customer balances without logging into the full ERP interface
- **Finance Teams** — audit bank accounts, categories, and financial contracts using natural language
- **Sales Reps** — check customer fiscal details and product availability during negotiations
- **Accounting Operations** — verify NF-e statuses and reconcile billing logs directly from the workspace


## Available Tools (15)
- **list_customers**: Listar base de clientes paginada extraindo entidades corporativas no ERP
- **get_customer**: Extrair perfil estático financeiro via UUID rastreando limites PF/PJ explícitos
- **search_customers**: Pesquisar perfis corporativos/fiscais comparando documentos restritos via CPF/CNPJ
- **create_customer**: Injetar novo registro financeiro PF/PJ definindo estrutura formal dentro do ERP
- **list_products**: Mapear itens físicos catalogados incluindo valores de SKU extraídos estaticamente
- **get_product**: Ler dados de um item físico individual incluindo limite e unidade de medida
- **create_product**: Mapear bens tangíveis definindo novos componentes faturáveis em Real financeiro
- **list_services**: Ler prestação categorizada cobrável na estrutura contábil faturada paginada
- **create_service**: Inserir prestação ativa intangível estritamente precificada na contabilidade
- **list_sales**: Listar logs contínuos extraídos avaliando faturas pendentes emitidas no fluxo
- **get_sale**: Visualizar blocos confirmados incluindo matrizes exatas contábeis da venda UUID
- **list_contracts**: Pesquisar recorrências atestando acordos automáticos limitando vencimentos
- **list_nfe**: Buscar listagem governamental acoplada de emissões NF (Notas de Produto)
- **list_categories**: g. Despesas, Receitas) que formam a espinha dorsal de DRE validada base ContaAzul.

Determinar limites contábeis de Plano Analítico nativo classificando recursos
- **list_bank_accounts**: Mapear bancos físicos conciliando integração extraindo posições monetárias


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conta Azul** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for customer with CNPJ '12.345.678/0001-90'"

**🤖 AI Agent:**
> I found the customer: 'Acme Brasil Ltda'. Their account is active, and they have 2 pending sales orders. Would you like to see their full financial history?

---

**👤 You:**
> "List the last 5 sales"

**🤖 AI Agent:**
> Here are the 5 most recent sales. The latest is Sale #982 for R$ 1.250,00 (Customer: John Doe). Status: Invoiced. I can retrieve the detailed accounting matrix for any of these.

---

**👤 You:**
> "Check the status of my NF-e emissions for this month"

**🤖 AI Agent:**
> Retrieving NF-e records... I found 12 product invoices issued this month. 11 are 'Approved by SEFAZ' and 1 is 'Pending'. Would you like to see the details for the pending invoice?


## ❓ FAQ

**Q: Can my agent search for customers using Brazilian documents like CPF or CNPJ?**
Yes. The 'search_customers' tool performs iterative regex analysis on names and documents. You can provide a CPF or CNPJ string, and the agent will locate the exact match within your Conta Azul database.

**Q: How do I check the status of a specific product invoice (NF-e)?**
Use the 'list_nfe' tool. Your agent will sweep governmental emission records and validate the approval status with SEFAZ, ensuring you have real-time visibility into your fiscal compliance.

**Q: Can I monitor recurring contracts via the agent?**
Absolutely. The 'list_contracts' tool captures financial limits for monthly or annual agreements, allowing your agent to detail continuous links and track expiration dates without generating instant fiscal documents.

**Q: How do I check my available bank balance?**
Use the 'list_bank_accounts' tool. Your agent will retrieve the real-time balance for all integrated accounts in your Conta Azul workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conta-azul](https://vinkius.com/mcp/conta-azul)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conta Azul** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conta-azul` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conta Azul** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conta-azul": {
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
