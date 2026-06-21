# Lexware Office (Accounting & Invoicing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lexware-office-accounting-invoicing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage bookkeeping via Lexware Office (lexoffice) — create contacts, track invoices, and audit accounting vouchers in Germany.

## Description
Connect your **Lexware Office (lexoffice)** account to any AI agent and take full control of your cloud-based accounting and invoicing through natural conversation.

### What you can do

- **Contact Management** — List and structure all business contacts (customers, vendors) and create new records with precise role assignments directly from your agent
- **Invoice Lifecycle** — Browse chronologically sorted invoices and retrieve detailed line items, VAT breakdowns, and payment statuses securely
- **Accounting Vouchers** — Access a unified stream of all recorded vouchers, including expenses, revenue, and credit notes for easy bookkeeping audits
- **Sales Pipeline** — List and inspect quotations, order confirmations, and delivery notes to monitor your sales and logistics workflow
- **Financial Configuration** — Query global payment conditions and posting categories to ensure accurate account mapping and tax compliance
- **Credit Notes Audit** — Retrieve exact amount details and positions for credit notes to manage cancellations and financial corrections efficiently

### How it works

1. Subscribe to this server
2. Enter your Lexware Office API Key
3. Start managing your bookkeeping from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners in Germany** — monitor outstanding payments and manage customer master data through natural conversation
- **Freelancers** — track invoices and expenses without leaving your development or design environment
- **Accountants & Ops** — audit voucher categories and tax mappings to ensure GoBD compliance across the entire accounting system


## Available Tools
- **list_contacts**: Nützlich zur Verwaltung der Stammdaten.

Alle Kontakte (Kunden, Lieferanten) in Lexoffice strukturieren und auflisten
- **get_contact**: Detaillierte Kontaktinformationen eines Kunden oder Lieferanten abrufen
- **create_contact**: Berücksichtigt hierbei standardisierte Formatierung für Kontaktpersonen (Vorname Nachname) und Rollenzuweisungen.

Neuen Geschäftsdatensatz (Kunde oder Lieferant) in Lexoffice anlegen
- **list_invoices**: Verwendet standardmäßig die paginierte Ansicht.

Alle abgerechneten Rechnungen auflisten, chronologisch sortiert
- **get_invoice**: -Beträge (Steuer), Netto-/Bruttosummen sowie Statusverknüpfungen (bezahlt, offen, mahnend).

Detaillierte Informationen sowie Positionen einer bestimmten Rechnung abrufen
- **list_credit_notes**: Gutschriftsbelegen zur buchhalterischen Prüfung nach Datum absteigend strukturiert.

Historie aller in Lexoffice verzeichneten Gutschriften anzeigen
- **get_credit_note**: Exakte Betragsdetails und Positionen einer spezifischen Gutschrift abfragen
- **list_quotations**: Zusammenstellung offener und abgeschlossener Angebote auflisten
- **get_quotation**: Umfangreiche Einzelheiten (Beträge, Positionen) eines bestimmten Angebots betrachten
- **list_order_confirmations**: Strukturiertes Register aller bisherigen Auftragsbestätigungen aufrufen
- **list_delivery_notes**: Sammlung ausgestellter Lieferscheine (Versanddokumente) abrufen
- **list_vouchers**: Deckt Rechnungen, Gutschriften und Ausgaben in einem gebündelten Datenstrom ab.

Gesamtübersicht aller Arten verbuchter Belege (Ausgaben, Einnahmen) betrachten
- **list_payment_conditions**: Stammdaten zu global hinterlegten Zahlungsbedingungen (Zahlungsziele, Skonto) abfragen
- **list_posting_categories**: Dies regelt in der Zuordnung, auf welches DATEV- oder Interne-Konto ein Vorfall verbucht wird.

Definierte Buchungskategorien / Kontorahmen für Einnahmen und Ausgaben anzeigen


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lexware Office (Accounting & Invoicing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices from Lexware Office"

**🤖 AI Agent:**
> I've retrieved the latest 5 invoices. Highlights include RE-1001 (€1,200, Paid), RE-1002 (€450, Open), and RE-1003 (€2,100, Overdue). Would you like to see the detailed line items for any of these?

---

**👤 You:**
> "Show me the details for contact 'TechGmbH' (ID: cont-123)"

**🤖 AI Agent:**
> Contact 'TechGmbH' (ID: cont-123) is registered as a CUSTOMER. Their primary address is in Berlin, and they have 12 total invoices with no outstanding balance. Their primary email is billing@techgmbh.de.

---

**👤 You:**
> "What are my current payment conditions?"

**🤖 AI Agent:**
> I've identified 3 active payment conditions: 1) 'Immediate' (due on receipt), 2) '14 Days' (standard), and 3) '30 Days Net'. I can provide the specific UUIDs if you need to create a new invoice.


## ❓ FAQ

**Q: Can I create a new customer record through my agent?**
Yes. Use the `create_contact` tool by providing the company name, contact person, and email. Your agent will format the data according to Lexware Office standards and assign the correct role ('customer' or 'vendor') instantly.

**Q: How do I check the payment status of an invoice?**
The `get_invoice` tool retrieves the complete document structure, including the current status (e.g., 'paid', 'open', or 'overdue'). Your agent can summarize these details for you directly in the conversation.

**Q: Can my agent list all accounting categories available in my account?**
Absolutely. Use the `list_posting_categories` tool to retrieve the defined chart of accounts. This is essential for understanding how revenues and expenses are mapped to your financial reports and DATEV exports.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lexware-office-accounting-invoicing](https://vinkius.com/mcp/lexware-office-accounting-invoicing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lexware Office (Accounting & Invoicing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lexware-office-accounting-invoicing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lexware Office (Accounting & Invoicing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lexware-office-accounting-invoicing": {
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
