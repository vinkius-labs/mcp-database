# Amazon Bedrock KB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-bedrock-kb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect your AI agent to AWS Bedrock Knowledge Bases — execute semantic searches, managed RAG, and sync vector datasources natively.

## Description
Connect your **Amazon Bedrock** account to any AI agent and empower it with managed vector databases, enterprise RAG workflows, and semantic search directly inside AWS.

### What you can do

- **Managed RAG** — Generate grounded LLM responses using internal document sets in a single explicit call
- **Semantic Retrieval** — Query vector indexes to retrieve exact top-K text chunks and their origin document URLs
- **Data Sources** — Inspect and paginate attached storage buckets feeding the knowledge base
- **Ingestion Jobs** — Track real-time syncing status of chunking pipelines mapping documents across the vector layout
- **Knowledge Base Introspection** — List available vector stores and exact embedding models assigned directly to your region

### How it works

1. Subscribe to this server
2. Enter your AWS IAM Role/User Access Credentials
3. Start augmenting your agent's context from Claude, Cursor, or any MCP-compatible client

Eliminate the need to build custom vector pipelines. Your agent queries massive corporate datasets precisely where they reside in AWS.

### Who is this for?

- **AI Developers** — build RAG workflows rapidly without hosting databases or maintaining chunking sync logic
- **Cloud Architects** — audit ingestion status and check origin document mappings securely from your chat interface
- **Data Scientists** — prototype context-grounded queries instantly and trace accuracy against exact data chunks


## Available Tools
- **list_knowledge_bases**: List AWS Bedrock knowledge bases
- **get_knowledge_base**: Get an explicit AWS Bedrock knowledge base
- **retrieve**: Query a vector index securely via AWS Bedrock
- **retrieve_and_generate**: Generate explicitly grounded LLM responses using Bedrock KB
- **list_data_sources**: List Data Sources bound explicitly to an AWS Bedrock KB
- **list_ingestion_jobs**: List AWS Bedrock KB explicit sync operations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon Bedrock KB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which knowledge bases and embedding models do I have setup?"

**🤖 AI Agent:**
> You have 1 Knowledge Base matching your region: 'Internal Wiki KB' (ID: ABCDE12345). It is mapped to the standard AWS Titan Text v2 embedding model and active for incoming syncs.

---

**👤 You:**
> "Run a retrieval query for 'onboarding process checklist' on my KB and show me the top 3 snippets."

**🤖 AI Agent:**
> I retrieved 3 matches from your KB. Segment 1 (from s3://hr-docs/onboarding.pdf) states: 'Ensure HR syncs Slack accounts within 24h...' Segment 2 (from s3://hr-docs/it-protocols.docx) mentions hardware issuance. Segment 3 highlights the welcome email template.

---

**👤 You:**
> "Check the status of the S3 ingestion job for my Documentation bucket."

**🤖 AI Agent:**
> The ingestion job for Data Source ID XYZ098 on Knowledge Base ABCDE12345 completed successfully today at 08h30. 15 new documents were chunked and mapped to the index without errors.


## ❓ FAQ

**Q: Can my AI agent directly run RAG without calling external LLMs?**
Yes! Use the `retrieve_and_generate` capability. Your agent passes the query and a designated Bedrock model ARN. Bedrock handles fetching chunks from the local vector index and synthesizing the final answer inside AWS boundaries, returning a fully grounded response instantly.

**Q: How can I check if new uploaded documents are successfully indexed in my agent?**
Just ask your agent to list ingestion jobs for a specific Knowledge Base ID and Data Source ID. It will report back the exact status (e.g., SYNCING, COMPLETED, FAILED) of chunks being mapped to your vector layout.

**Q: Can I see exactly where an answer came from in my documentation?**
Absolutely. Both the standard `retrieve` functionality and `retrieve_and_generate` calls will parse out the specific origin document URLs (e.g., S3 paths) and expose the exact raw text snippets that mathematically matched your query vector.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-bedrock-kb](https://vinkius.com/mcp/amazon-bedrock-kb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amazon Bedrock KB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amazon-bedrock-kb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amazon Bedrock KB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amazon-bedrock-kb": {
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
