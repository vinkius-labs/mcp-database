# Mastercard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mastercard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Identify cards, validate accounts, find merchants, and detect fraud via Mastercard payment APIs.

## Description
Connect **Mastercard** payment infrastructure to any AI agent and unlock powerful payment intelligence, fraud detection, merchant discovery, and card validation capabilities through natural conversation.

### What you can do

- **BIN Lookup** — Identify any payment card's issuer bank, card type (credit/debit/prepaid/commercial), category (Standard/Gold/Platinum/World/World Elite), issuing country, and special flags from just the first 6-8 digits
- **Account Validation** — Verify if a payment card number is active and valid before processing transactions, reducing declined payments and fraud risk
- **Merchant Search** — Find Mastercard-accepting merchants near any GPS coordinates, filterable by business category (MCC codes)
- **Places Discovery** — Discover nearby payment-accepting locations with digital wallet support (Apple Pay, Google Pay, contactless)
- **Address-Based Search** — Search for merchants by street address instead of coordinates for user-friendly location queries
- **Merchant Details** — Retrieve complete information about specific merchants including addresses, MCC codes, and accepted payment methods
- **MCC Code Reference** — Access the complete Merchant Category Code database to understand business classifications
- **Fraud Reporting** — Submit confirmed fraudulent transactions to Mastercard's Fraud and Loss Database to protect the network
- **Nearby Locations** — Discover ATMs, merchants, and points of interest around any geographic location

### How it works

1. Subscribe to this server
2. Enter your Mastercard Developers Client ID and Client Secret
3. Start querying payment intelligence from Claude, Cursor, or any MCP-compatible client

Your AI acts as a payment infrastructure assistant — no more navigating complex payment portals or writing custom API integrations. Get instant answers about cards, merchants, and transactions.

### Who is this for?

- **Fintech Developers** — validate cards, identify BINs, and reduce transaction declines by verifying accounts before processing payments
- **Fraud Analysts** — quickly look up card issuer details, submit confirmed fraud reports, and investigate suspicious transactions through conversational AI
- **Travel & Concierge Services** — find nearby merchants, discover payment-accepting locations with Apple Pay support, and help travelers understand local payment infrastructure
- **E-commerce Operators** — identify card types before checkout to optimize payment routing, detect prepaid/commercial cards, and reduce cross-border processing fees


## Available Tools
- **bin_lookup**: Returns comprehensive card information including: issuer bank name, card type (credit/debit/prepaid/commercial), card category (Standard/Gold/Platinum/World/World Elite), issuing country, currency, and special flags (healthcare, payroll, purchasing). Use this to identify unknown cards, validate card ranges before transactions, determine cross-border fees, or understand the cardholder profile. The accountNumberPrefix parameter must be 6-8 numeric digits. Optional parameters (currencyCode, paymentType, merchantCategoryCode) provide more precise results for specific transaction contexts.

Identify card issuer, type, and details from the first 6-8 digits of a payment card number
- **bin_lookup_post**: Returns identical card identification data: issuer bank, card type, category, country, and product flags. Use this method when handling sensitive payment data in compliance-focused applications. The accountNumberPrefix should be 6-8 digits. Optional context parameters (currency, payment type, MCC) refine results.

Identify card issuer using POST method for enhanced security with sensitive card data
- **get_merchant**: Returns full address, contact information, MCC code, operating hours, and accepted payment methods. Use this to get in-depth information about a specific merchant location after finding it via search. The merchant ID is a unique identifier returned by the search_merchants tool.

Get detailed information about a specific Mastercard-accepting merchant
- **get_place_details**: Returns full address, coordinates, MCC code, payment methods accepted, operating hours, and other merchant attributes. Use this after a places search to drill down into a specific location. The locationId is returned by search_places or search_places_by_address tools.

Get complete details for a specific merchant place by its location ID
- **merchant_category_codes**: MCC codes are 4-digit numbers that classify businesses by type (e.g., 5411 = Grocery Stores, 5812 = Restaurants, 4511 = Airlines). Use this to understand merchant classifications, filter searches by business type, or decode MCC values found in transaction data. Optional limit parameter controls how many codes to return.

List all Merchant Category Codes (MCC) used to classify business types
- **merchant_industry_codes**: Industry codes group related MCC codes into higher-level categories. Use this to understand the hierarchical classification of merchants, analyze industry-level spending patterns, or build category navigation interfaces.

List all merchant industry codes for broader business classification
- **nearby_locations**: Returns names, addresses, categories, and distances from the search point. Use this for "what is nearby" queries, travel planning, or finding payment infrastructure in an area. Latitude and longitude are required. Radius in meters defines the search area. Limit controls maximum results returned.

Discover points of interest and payment locations near GPS coordinates
- **search_merchants**: Returns merchant names, addresses, MCC codes, and precise coordinates. Use this to find nearby payment-accepting locations, analyze merchant density in an area, or build "find merchants near me" features. Latitude and longitude are required as strings (e.g., "-23.5505", "-46.6333"). Radius is in meters (e.g., 5000 for 5km). Optionally filter by MCC category code (e.g., "5411" for grocery stores, "5812" for restaurants). Limit controls result count (max 50).

Find Mastercard-accepting merchants near specific GPS coordinates filtered by category
- **search_places**: Returns detailed merchant information including whether they accept Apple Pay, Google Pay, contactless payments, and their MCC classification. Use this when users need to find payment-accepting locations with specific digital wallet support. Latitude and longitude are required as numbers. Distance is in kilometers. Optionally filter by country code (ISO 3166-1 alpha-2) and payment capabilities (hasApplePay, hasGooglePay).

Search for merchant places using GPS coordinates with payment method filters
- **search_places_by_address**: The API geocodes the address internally. Returns nearby merchants with payment capability details (Apple Pay, Google Pay, contactless). Use this when users provide an address rather than GPS coordinates. Required: address line 1, city, country code, and postal code. Optional: state/province code (countrySubdivisionCode) for more precise results. Example: addressLine1="1600 Amphitheatre Pkwy", city="Mountain View", countryCode="US", postalCode="94043".

Search for merchant places using a street address instead of coordinates
- **submit_fraud_report**: This is a critical tool for issuers and processors to flag fraudulent transactions in real-time. Required fields: accountNumber (card number), transactionAmount, transactionCurrency (ISO 4217), and fraudTypeCode. Fraud type codes: "01" = Stolen Card Fraud, "02" = Never Received Card, "03" = Fraudulent Application, "04" = Counterfeit Card Fraud. Optional: fraudAmount (if different from transaction amount), transactionDate (YYYY-MM-DD). Use this only for confirmed fraud cases — never for suspected or disputed transactions. This helps Mastercard improve fraud detection and reduce false positives across the network. IMPORTANT: This action should only be performed by authorized fraud management personnel.

Report a confirmed fraudulent transaction to Mastercard Fraud and Loss Database
- **validate_account**: Returns validation status (VALID/INVALID), account type, and issuer information. Use this to verify card validity before processing transactions, reduce declined transactions, or perform account verification during onboarding. Required: accountNumber (full card number). Optional: expiryDate (MMYY format), cardholderName for enhanced validation. Handle card numbers securely — never log or store full PANs.

Validate a payment card account number to check if it is active and valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mastercard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What type of card is 542418 and which bank issued it?"

**🤖 AI Agent:**
> Running BIN lookup for 542418... This is a Mastercard World Elite credit card issued by Banco Exemplo S.A. in Brazil. It's a premium tier card (not prepaid, not commercial) with BRL as the primary currency. The BIN range covers 54241800 to 54241899.

---

**👤 You:**
> "Find restaurants near São Paulo city center that accept Mastercard within 3km."

**🤖 AI Agent:**
> Found 27 restaurants within 3km of São Paulo center. Top results include: Restaurante Paulista (MCC: 5812) at Av. Paulista, 500; Sabor Brasileiro on Rua Augusta, 1200; and Pizzaria Bella on Rua Oscar Freire, 800. All accept Mastercard. Would you like details on any specific restaurant?

---

**👤 You:**
> "Validate card number 5123456789012346 before I process this payment."

**🤖 AI Agent:**
> Card validation complete: ****2346 is VALID. Account type: Credit card. Issuer: First National Bank. The card is active and ready for transactions. You can proceed with processing this payment safely.


## ❓ FAQ

**Q: Can I identify what bank issued a card just from the first few digits?**
Yes! Use the `bin_lookup` tool with the first 6-8 digits of the card number (the BIN). Mastercard will return the issuer bank name, card type (credit/debit/prepaid), card category (Gold/Platinum/World), issuing country, and flags like whether it's a commercial or healthcare card. For example, BIN 542418 reveals the exact issuing bank and card tier.

**Q: How can I find merchants that accept Mastercard near a specific location?**
Use the `search_merchants` tool with latitude, longitude, and a search radius in meters. You can optionally filter by MCC code (e.g., "5812" for restaurants, "5411" for grocery stores). For example, searching with coordinates -23.5505, -46.6333 (São Paulo) and radius 5000 will return all Mastercard-accepting merchants within 5km. Results include merchant names, addresses, categories, and coordinates.

**Q: Can I verify if a payment card is valid before processing a transaction?**
Yes! Use the `validate_account` tool with the full card number. It checks Mastercard records to determine if the card is active and valid, returning the validation status (VALID/INVALID), account type (credit/debit/prepaid), and issuer information. Optionally include expiry date (MMYY format) and cardholder name for enhanced validation. This helps reduce declined transactions and fraud risk. Never store full card numbers — handle them securely.

**Q: How do I report a confirmed fraudulent transaction to Mastercard?**
Use the `submit_fraud_report` tool with the card number, transaction amount, currency (ISO 4217), and fraud type code. Fraud types: "01" = Stolen Card, "02" = Never Received Card, "03" = Fraudulent Application, "04" = Counterfeit Card. Optionally include fraud amount and transaction date. This submits to Mastercard's Fraud and Loss Database (FLD) to help reduce false positives across the network. IMPORTANT: Only authorized fraud management personnel should use this tool for confirmed cases.

**Q: Can I find merchants that accept Apple Pay or Google Pay near me?**
Yes! Use the `search_places` tool with GPS coordinates and set hasApplePay=true or hasGooglePay=true to filter for merchants with those payment capabilities. Returns detailed merchant information including names, addresses, MCC codes, and which digital wallets they accept. For example, searching near Times Square (40.7580, -73.9855) with hasApplePay=true will show all nearby Apple Pay-enabled merchants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mastercard](https://vinkius.com/mcp/mastercard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mastercard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mastercard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mastercard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mastercard": {
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
