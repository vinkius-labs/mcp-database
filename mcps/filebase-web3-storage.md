# Filebase (Web3 Storage) MCP Server

Manage decentralized storage on IPFS via Filebase — upload files, pin CIDs, manage IPNS names, and track storage usage directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/filebase-web3-storage)

## Overview
**Category:** developer-tools
**Tools Count:** 29

## Description
Connect your **Filebase** account to any AI agent and take full control of your decentralized Web3 storage workflows through natural conversation.

### What you can do

- **IPFS Operations** — Add text files, fetch content by CID, and manage raw blocks directly on the IPFS network using the RPC API.
- **Pinning Management** — Use the Pinning Service API (PSA) or RPC to pin, list, and remove content identifiers (CIDs) for persistent storage.
- **IPNS & Keys** — Generate keypairs, publish CIDs to IPNS, and resolve names to IPFS paths for mutable decentralized websites.
- **Usage & Infrastructure** — Monitor storage usage, manage dedicated gateways, and track bucket metrics across the platform.

### How it works

1. Subscribe to this server
2. Enter your Filebase API Key and Platform Token
3. Start managing your Web3 assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — interact with IPFS and IPNS directly from your coding environment without switching to CLI or web dashboards.
- **DevOps Engineers** — automate pinning and storage monitoring as part of your infrastructure workflows.
- **Content Creators** — manage decentralized assets and metadata for NFTs or dApps using simple natural language commands.


## Available Tools
- **platform_create_gateway**: Create a new dedicated gateway
- **platform_create_name**: Create a new IPNS name
- **platform_delete_gateway**: Delete a dedicated gateway
- **platform_delete_name**: Delete an IPNS name
- **platform_get_bucket_usage**: Get storage usage for a specific bucket
- **platform_get_gateway**: Get details of a specific dedicated gateway
- **platform_get_gateway_usage**: Get bandwidth usage for a dedicated gateway
- **platform_get_name**: Get details of a specific IPNS name
- **platform_get_usage**: Get total storage and bandwidth usage
- **platform_list_gateways**: List all dedicated gateways
- **platform_list_names**: List all IPNS names
- **platform_update_gateway**: Update a dedicated gateway
- **platform_update_name**: Update an IPNS name to point to a new CID
- **psa_add_pin**: Add a pin using the Pinning Service API
- **psa_get_pin**: Get pin status by request ID
- **psa_list_pins**: List pins using the Pinning Service API
- **psa_remove_pin**: Remove a pin by request ID
- **psa_replace_pin**: Replace an existing pin
- **rpc_add**: Add a text file to IPFS
- **rpc_block_get**: Retrieve a raw block by CID
- **rpc_cat**: Fetch contents of a file by CID
- **rpc_key_gen**: Create a new keypair
- **rpc_key_list**: List all keys in the keychain
- **rpc_name_publish**: Publish a CID to IPNS
- **rpc_name_resolve**: Resolve an IPNS name to an IPFS path
- **rpc_pin_add**: Pin a CID to persistent storage
- **rpc_pin_ls**: List all pinned objects via RPC
- **rpc_pin_rm**: Unpin a CID via RPC
- **rpc_version**: Get the version of the IPFS daemon


## Installation & Usage

To install and use the **Filebase (Web3 Storage)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filebase-web3-storage](https://vinkius.com/mcp/filebase-web3-storage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
