# Sablier (Token Streaming & Real-time Payroll) MCP Server

Manage real-time token streams and airdrop campaigns. Query Sablier indexers, create Merkle trees for distributions, and check wallet eligibility.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sablier-token-streaming-real-time-payroll)

## Overview
**Category:** finance-accounting
**Tools Count:** 4

## Description
Connect your **Sablier** protocol data to any AI agent to manage real-time finance, payroll, and token distributions through natural language.

### What you can do

- **Stream Analysis** — Query Lockup and Flow streams directly from Envio or The Graph indexers using GraphQL.
- **Airdrop Management** — Create Merkle trees for token distributions by simply providing a CSV list of recipients and amounts.
- **Eligibility Verification** — Instantly check if a specific wallet address is eligible for an airdrop campaign using its IPFS CID.
- **Campaign Validation** — Verify that an IPFS CID points to a valid Sablier campaign configuration before interacting.

### How it works

1. Subscribe to this server
2. Provide your Sablier GraphQL URL and Merkle API URL
3. Start managing your on-chain payroll and distributions from Claude, Cursor, or any MCP client

### Who is this for?

- **DAO Operations** — Automate the checking of contributor stream statuses and manage large-scale distributions.
- **Web3 HR & Finance** — Monitor real-time payroll streams and validate airdrop eligibility for team members.
- **DeFi Power Users** — Query complex stream data and prepare Merkle campaigns without manual script writing.


## Available Tools
- **check_eligibility**: Check if an address is eligible for a campaign
- **check_validity**: Validate an IPFS CID for a Sablier campaign
- **create_merkle_campaign**: Returns the CID and Merkle root.

Create a new Merkle tree for an airdrop campaign
- **query_graphql**: Query Sablier streams and airdrops via GraphQL


## Installation & Usage

To install and use the **Sablier (Token Streaming & Real-time Payroll)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sablier-token-streaming-real-time-payroll](https://vinkius.com/mcp/sablier-token-streaming-real-time-payroll)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
