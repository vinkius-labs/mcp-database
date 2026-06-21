# Lexware Office (Accounting & Invoicing) MCP Server

Manage bookkeeping via Lexware Office (lexoffice) — create contacts, track invoices, and audit accounting vouchers in Germany.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lexware-office-accounting-invoicing)

## Overview
**Category:** finance-accounting
**Tools Count:** 14

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


## Installation & Usage

To install and use the **Lexware Office (Accounting & Invoicing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lexware-office-accounting-invoicing](https://vinkius.com/mcp/lexware-office-accounting-invoicing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
