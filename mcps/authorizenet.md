# Authorize.net MCP Server

Process cards, manage refunds, capture holds, and inspect settled transactions on Authorize.net directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/authorizenet)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your **Authorize.net** merchant gateway to any AI agent to power conversational commerce. Command precise payment logic, track settlements, and manage Customer Information Manager (CIM) profiles effortlessly.

### What you can do

- **Payment Processing** — Run strict "Auth & Capture" to process real funds instantly, or perform "Auth Only" to hold funds legitimately before shipping
- **Refunds & Voids** — Initiate refunds on previously settled transactions or Void anomalies residing in your pending batches cleanly
- **Vault & CIM Profiles** — Securely construct isolated Customer Information Profiles linking sensitive card data without exposing raw PANs to unencrypted bounds
- **Auditing & Settlements** — Query distinct details of a single transaction ID or map an overarching list of today's unsettled nightly batch runs

### How it works

1. Subscribe to this secure MCP Server
2. Add your Authorize.net Login ID, Transaction Key, and Environment mapping
3. Engage directly with Authorize.net's API via Claude, Cursor, or any compatible AI client

Your AI agent eliminates the clunky Merchant Interface, managing daily financial anomalies in pure dialogue.

### Who is this for?

- **E-Commerce Managers** — seamlessly execute post-return refunds dynamically on the fly
- **Sales Engineers** — verify exactly why a card was declined (AVS or CVV logic flaws) natively
- **Financial Ops** — track unresolved unsettled holds systematically prior to batch processing


## Available Tools
- **add_payment_profile**: Add a payment card to an existing CIM customer profile
- **auth_capture_transaction**: Perform an Authorize.net authorization and capture transaction
- **auth_only_transaction**: Place a temporary authorization hold on a credit card
- **prior_auth_capture**: Capture a previously authorized transaction hold
- **create_customer_profile**: net before securely attaching payment cards.

Create a new Customer Information Manager (CIM) profile
- **get_customer_profile**: Retrieve details of a Customer Information Manager (CIM) profile
- **get_transaction_details**: Get comprehensive details of a specific gateway transaction
- **get_unsettled_transactions**: List all unsettled transactions pending batch closure
- **refund_transaction**: You must pass the original transaction ID, the refund amount, and the original masked or raw PAN and expiration.

Refund an already settled Authorize.net transaction
- **void_transaction**: Void an unsettled Authorize.net transaction


## Installation & Usage

To install and use the **Authorize.net** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/authorizenet](https://vinkius.com/mcp/authorizenet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
