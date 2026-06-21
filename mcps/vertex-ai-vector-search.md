# Vertex AI Vector Search MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vertex-ai-vector-search)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vertex-ai-vector-search-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vertex-ai-vector-search-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Bring Google's massive vector matching power to your AI agent. Search billions of semantic embeddings and administer Vertex Index endpoints directly in chat.

## Description
Plug the sheer matching scale of Google Cloud's **Vertex AI Vector Search** directly into your intelligent IDE or conversational agent. Unleash low-latency nearest neighbor lookups across billion-scale embedding structures without navigating Cloud Console interfaces.

### What you can do

- **Massive Semantic Extraction** — Prompt your agent to formulate query vectors and blast them at your specialized Cloud endpoints. It instantly retrieves identical geometric text boundaries (nearest neighbors) to ground LLM contexts powerfully.
- **Index Operations** — Gain total situational awareness over your massive datasets. Command the bot to list your provisioned Vector Indexes, verifying dimensionality, configuration updates, and current active states within seconds.
- **Endpoint Monitoring** — List active network endpoints scaling your specific RAG applications. Determine clearly which underlying deployed index iterations are currently receiving production traffic without digging through IAM screens.
- **Operation Tracking** — Spun up a multi-terabyte index build? Query the cloud queue using chat to review persistent long-running task timelines from your primary editor.

### How it works

1. Enable the Google Cloud Vertex AI API for your project
2. Gather your Project ID, desired Location, and OAuth2 Access Token
3. Start fetching and comparing dense geometrical data structures conversationally

### Who is this for?

- **Cloud Machine Learning Ops (MLOps)** — check on multi-hour index deployment progression strictly through chat checks while continuing your Python scripting.
- **RAG Data Scientists** — quickly push experimental float arrays straight into production endpoints via Cursor, gauging proximity precision on-the-fly.
- **Backend Architects** — verify the infrastructure configuration, shards, and node counts tied to critical vector databases deployed organization-wide.


## Available Tools
- **get_index_details**: Retrieves metadata and configuration for a specific vector index
- **list_deployed_indexes**: Lists all indexes deployed to a specific endpoint
- **list_index_endpoints**: Lists all index endpoints in the project
- **list_vector_indexes**: Lists all vector indexes in the Google Cloud project
- **list_vector_operations**: Lists long-running operations related to vector indexes
- **search_nearest_neighbors**: Provide the endpoint ID, deployed index ID, and a query vector as a JSON array.

Performs a nearest neighbor vector similarity search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vertex AI Vector Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active vector indexes on the current GCP project."

**🤖 AI Agent:**
> I've scanned your infrastructure on Vertex AI. You currently have 2 core vector indexes active:
- `product_catalog_dense` (ID: 4858..., Dimensions: 768)
- `document_vault_prod` (ID: 3959..., Dimensions: 1536)

Would you like me to inspect endpoints verifying which of these are currently exposed for search?

---

**👤 You:**
> "Check for any long-running vector deployment operations currently uncompleted."

**🤖 AI Agent:**
> I've queried the Vertex AI Operations log.

There is currently `1` pending operation:
- **Operation ID**: `74803923`
- **Target**: Deploying index `document_vault_prod` to endpoint `112xyz`.
- **Status**: `RUNNING` (Approx 45% completion, started 22 minutes ago).

No errors or stalling reported on your cluster. I can poll this periodically if you wish.

---

**👤 You:**
> "Find the 3 nearest neighbors mapping to endpoint '39xl' array index ID 'dep_30' using vector [-0.2, 0.5, 0.0]."

**🤖 AI Agent:**
> I've passed the floating-point vector directly to the Vertex instance. The semantic similarities fetched from `dep_30` are:
1. Base ID `prod-281x` (Distance: 0.12)
2. Base ID `prod-994y` (Distance: 0.17)
3. Base ID `prod-110m` (Distance: 0.31)

This indicates extremely tight clustering to item *#281x* in the embedding space.


## Installation & Usage

To install and use the **Vertex AI Vector Search** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vertex-ai-vector-search](https://vinkius.com/mcp/vertex-ai-vector-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
