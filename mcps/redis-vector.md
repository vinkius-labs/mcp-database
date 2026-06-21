# Redis Vector MCP Server

Equip your AI to autonomously manage embeddings, run KNN similarity searches, and administrate vector indexes natively inside your Redis stack.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/redis-vector)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

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


## Installation & Usage

To install and use the **Redis Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redis-vector](https://vinkius.com/mcp/redis-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
