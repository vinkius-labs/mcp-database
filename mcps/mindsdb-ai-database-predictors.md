# MindsDB (AI Database & Predictors) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mindsdb-ai-database-predictors)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage AI-powered data via MindsDB — execute SQL predictions, audit ML models, and connect data sources.

## Description
Connect your **MindsDB** instance to any AI agent and take full control of your machine learning workflows, automated predictions, and data integrations through natural SQL-based conversation.

### What you can do

- **Predictive Orchestration** — Execute arbitrary SQL statements to trigger automated machine learning commands, including 'CREATE MODEL' and 'SELECT ... PREDICT' directly from your agent
- **Model Lifecycle Audit** — List trained AI tables (models) across your projects and retrieve detailed meta-features tracking generation progress or internal accuracy metrics
- **Data Source Integration** — Enumerate external databases connected through MindsDB (e.g., PostgreSQL, Snowflake, ClickHouse) to audit your data pipeline boundaries securely
- **Virtual View Management** — List virtual data views and SQL structural mappings that act as proxy tables for complex data transformation logic
- **Cluster Diagnostics** — Retrieve active cluster status and version statistics to verify the availability and health of your MindsDB environment
- **Advanced SQL Execution** — Run sophisticated queries combining scalar data with ML predictions to fetch literal insights across any schema entity natively

### How it works

1. Subscribe to this server
2. Enter your MindsDB API URL and API Key (if using Cloud)
3. Start automating your machine learning from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — test predictor accuracy and monitor ML model training statuses through natural conversation without manual CLI tools
- **Software Developers** — integrate AI-powered predictions into applications and verify data source connections directly from your workspace
- **BI Analysts** — execute SQL queries that combine historical data with future predictions to generate rapid business insights efficiently


## Available Tools (6)
- **list_databases**: List external databases connected through MindsDB
- **list_models**: Use when checking which algorithms are ready to query predictions.

List trained AI tables (models) available in a project
- **get_model**: Get an explicitly trained AI prediction engine
- **execute_sql_query**: E.g: CREATE DATABASE, SELECT ... WHERE, CREATE MODEL ... PREDICT. Wrap logic safely. VERY IMPORTANT: queries returning a large number of rows MUST be explicitly wrapped in a LIMIT statement or risk hitting context overflow.

Execute arbitrary SQL statements bounding MindsDB elements
- **list_views**: List virtual data views stored inside a target project
- **get_status**: Acts as a ping tracer returning valid core version/health specs.

Get active cluster diagnostic and version statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MindsDB (AI Database & Predictors)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ML models in the 'mindsdb' project"

**🤖 AI Agent:**
> I've retrieved your AI models from the 'mindsdb' project. Highlights include 'home_price_predictor' (Status: Complete), 'sales_forecaster' (Status: Training, 45%), and 'customer_churn_model'. Which one would you like to check the accuracy for?

---

**👤 You:**
> "Execute SQL: SELECT price, price_explain FROM mindsdb.home_price_predictor WHERE sqft = 2500"

**🤖 AI Agent:**
> Executing prediction query… The predicted price for a 2500 sqft home is $450,000. Explanation: The model heavily weighted the square footage and recent neighborhood sales trends. Would you like to run this prediction for a different set of features?

---

**👤 You:**
> "Show me all connected databases in my MindsDB instance"

**🤖 AI Agent:**
> I've identified 3 connected data sources: 'production_pg' (PostgreSQL), 'snowflake_warehouse' (Snowflake), and 'marketing_sheets' (Google Sheets). I can list the available tables for any of these sources if you'd like.


## ❓ FAQ

**Q: Can I train a machine learning model using SQL through my agent?**
Yes. Use the `execute_sql_query` tool with the 'CREATE MODEL' statement. Your agent will dispatch the command to MindsDB, which will automatically handle the data processing and training of your predictor asynchronously.

**Q: How do I connect an external database like PostgreSQL to MindsDB using the agent?**
The `execute_sql_query` tool supports the 'CREATE DATABASE' syntax. You can command your agent to link a new data source by providing the connection parameters, allowing MindsDB to query your existing data natively.

**Q: Can my agent retrieve the status of an ongoing model training?**
Absolutely. Use the `get_model` tool by providing the model name and project. Your agent will report the current training state, accuracy metrics, and any errors encountered during the AI generation process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mindsdb-ai-database-predictors](https://vinkius.com/mcp/mindsdb-ai-database-predictors)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MindsDB (AI Database & Predictors)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mindsdb-ai-database-predictors` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MindsDB (AI Database & Predictors)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mindsdb-ai-database-predictors": {
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
