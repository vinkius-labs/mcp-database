# Sablier (Token Streaming & Real-time Payroll) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sablier-token-streaming-real-time-payroll)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage real-time token streams and airdrop campaigns. Query Sablier indexers, create Merkle trees for distributions, and check wallet eligibility.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sablier (Token Streaming & Real-time Payroll)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if address 0x71C7656EC7ab88b098defB751B7401B5f6d8976F is eligible for the campaign with CID QmXoypizjW3WknFiJnKLwHCnL72vedxjQkDDP1mXWo6uco."

**🤖 AI Agent:**
> I've checked the eligibility for that address. It is eligible for the campaign! The claimable amount is 500 tokens.

---

**👤 You:**
> "Create a Merkle campaign for a token with 18 decimals using this CSV: address,amount
0x123...,100.5
0x456...,200"

**🤖 AI Agent:**
> The Merkle tree has been created and pinned to IPFS. The Merkle Root is 0xabc... and the IPFS CID is QmZ... You can now use this CID to initialize your Sablier campaign.

---

**👤 You:**
> "Query the Sablier indexer for all active FlowStreams where the sender is 0x5678..."

**🤖 AI Agent:**
> I found 3 active FlowStreams for that sender. Stream #101 is streaming USDC at a rate of 0.01 per second, and Stream #105 is streaming DAI.


## ❓ FAQ

**Q: How do I check if a user is eligible for a specific airdrop?**
Use the `check_eligibility` tool. You will need the user's wallet address and the IPFS CID of the Sablier campaign. The agent will query the Merkle API and return the eligibility status.

**Q: Can I create a new distribution list for an airdrop?**
Yes! The `create_merkle_campaign` tool allows you to upload raw CSV content (addresses and amounts). It will generate the Merkle tree, pin it to IPFS, and return the root and CID.

**Q: What data can I retrieve using the GraphQL tool?**
The `query_graphql` tool can fetch any data indexed by Sablier, including LockupStreams, FlowStreams, and Campaign details. You can filter by sender, recipient, or token address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sablier-token-streaming-real-time-payroll](https://vinkius.com/mcp/sablier-token-streaming-real-time-payroll)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sablier (Token Streaming & Real-time Payroll)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sablier-token-streaming-real-time-payroll` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sablier (Token Streaming & Real-time Payroll)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sablier-token-streaming-real-time-payroll": {
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
