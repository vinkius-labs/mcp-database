# Redis Vector MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/redis-vector)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/redis-vector-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/redis-vector-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Equip your AI to autonomously manage embeddings, run KNN similarity searches, and administrate vector indexes natively inside your Redis stack.

## Description
Connect your **Redis** database (equipped with the RediSearch module) to your AI agent, turning it into an advanced Vector Database administrator. Activating this integration grants your conversational interface the power to interact directly with your semantic search engine, enabling tasks like querying mathematical embeddings for similar records, configuring fresh vector indexes, and managing geometric data structures without needing dedicated external database clients.

### What you can do

- **Similarity Vector Search (KNN)** — Let the AI perform rapid native vector comparisons (`search_vectors`). Provide an embedding array via prompt or code, and retrieve the absolute nearest `top_k` neighbors securely cached in your infrastructure.
- **Index Management** — Actively discover all loaded RediSearch vector indexes, investigate their configured dimensions (`get_index_info`), or command the AI to instantiate new KNN indexes (`create_vector_index`) tailored for fresh AI workloads.
- **Embedding Administration** — Inject and modify geometric vector components associated with a document key (`upsert_vector`), or purge legacy embeddings efficiently (`delete_vector`) to keep semantic records clean and operational.

### How it works

1. Authorize the Redis Vector MCP connector from your module catalog.
2. Configure it securely by providing your full `Redis URL` (ensure it points to a Redis instance that natively supports RediSearch vector extensions).
3. Prompt your AI to "find the top 5 nearest neighbors for this JSON array in the 'products-index'" or "create a new 1536-dimensional vector index for OpenAI embeddings."

### Who is this for?

- **AI & ML Engineers** — Rapidly iterate over similarity tuning. Store resulting chunk embeddings on the fly, and query KNN vectors right from the prompt instead of scripting Python drivers repeatedly.
- **Backend Developers** — Maintain semantic storage logic. Audit schemas, map out active index properties, and delete obsolete hashes holding raw vector models instantly.
- **Data Architects** — Validate your Redis vector environments interactively. Explore dimension structures and index readiness confirming architecture viability for RAG (Retrieval-Augmented Generation) applications.


## Available Tools
- **create_vector_index**: Specify the name and vector dimensions.

Creates a new RediSearch vector index
- **delete_vector**: Deletes a vector document from Redis
- **get_index_info**: Retrieves details for a specific vector index
- **list_indexes**: Lists all RediSearch vector indexes
- **search_vectors**: Provide the query vector as a JSON array of floats.

Performs a KNN similarity search in a vector index
- **upsert_vector**: Specify the document key and the vector as a JSON array.

Inserts or updates a vector in a Redis hash


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Redis Vector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the index 'customer-support-vector' for the top 3 similar records to this embedding vector: [0.12, -0.45, 0.08, 0.99...]"

**🤖 AI Agent:**
> I processed the array using `search_vectors` on 'customer-support-vector'. Here are the 3 nearest key entries based on distance proximity:
1. doc:faq:882 (score: 0.89)
2. doc:faq:104 (score: 0.81)
3. doc:faq:002 (score: 0.77)

---

**👤 You:**
> "Insert a new embedding into the database with the key 'user:439:preference' containing the vector `[0.2, -0.1...]`."

**🤖 AI Agent:**
> Running `upsert_vector`... I have successfully saved the document 'user:439:preference' containing the provided embedding data matrix into Redis. It is now queryable.

---

**👤 You:**
> "Retrieve the index information logic and schema mapping for 'docs-semantic-index'."

**🤖 AI Agent:**
> I extracted the metadata using `get_index_info`. 'docs-semantic-index' holds 5,000 documents parameterized with the HNSW algorithm, set to 1536 float dimensions, utilizing the COSINE metric protocol.


## Installation & Usage

To install and use the **Redis Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redis-vector](https://vinkius.com/mcp/redis-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
