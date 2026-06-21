# Hotmart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hotmart-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Sell online courses, digital products, and memberships on the leading platform for digital creators in Latin America and beyond.

## Description
Connect your **Hotmart** account to any AI agent and manage your digital product business through natural conversation.

### What you can do

- **Product Catalog** — List all your digital products (courses, ebooks, memberships) with pricing and status
- **Sales History** — Browse all transactions with status, buyer details, and commission breakdowns
- **Revenue Summary** — Get aggregated sales data including total revenue, number of sales, and average ticket
- **Subscription Management** — List all active subscriptions with renewal dates and payment status
- **Student Tracking** — Browse all enrolled students and inspect individual course completion progress

### How it works

1. Subscribe to this server
2. Enter your Hotmart Client ID and Client Secret from the developer portal
3. Start managing your products from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Creators** — monitor product sales, track student engagement, and review revenue without opening the Hotmart dashboard
- **Course Authors** — check student progress, identify drop-off points, and manage subscriber lists
- **Affiliate Managers** — review sales commissions, track affiliate performance, and audit transaction histories


## Available Tools
- **get_sales_history**: Get sales history
- **get_sales_summary**: Get sales summary
- **get_student_progress**: Get progress for a student
- **list_products**: List all your products
- **list_students**: List students (members)
- **list_subscriptions**: List active subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotmart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all my products with sales data and the revenue summary for this month."

**🤖 AI Agent:**
> Your products: 1) 'AI Mastery Course' — R$ 297, Active, 1,240 total sales. 2) 'Python Bootcamp' — R$ 197, Active, 890 total sales. 3) 'Data Science eBook' — R$ 47, Active, 2,100 total sales. Revenue summary (April 2025): Total revenue: R$ 48,230. Number of sales: 312. Average ticket: R$ 154.58. Top performer: 'AI Mastery Course' (R$ 28,710, 58.5% of revenue). Active subscriptions: 89. Would you like to see the sales history or student progress?

---

**👤 You:**
> "Show student progress for the AI Mastery Course — who is falling behind?"

**🤖 AI Agent:**
> AI Mastery Course: 1,240 enrolled students. Completion breakdown: Completed (100%): 312 students (25.2%). Active (50-99%): 456 students (36.8%). At risk (10-49%): 289 students (23.3%). Inactive (<10%): 183 students (14.8%). Students falling behind (inactive >30 days): 1) Maria Silva (student_891) — 12% complete, last activity 45 days ago. 2) João Santos (student_902) — 8% complete, 38 days. 3) Ana Costa (student_915) — 22% complete, 35 days. Module with highest drop-off: Module 4 'Neural Networks' (42% abandon rate). Would you like to check subscriptions or get the full sales history?

---

**👤 You:**
> "Show the last 5 sales transactions and list all active subscriptions."

**🤖 AI Agent:**
> Last 5 sales: 1) 'AI Mastery Course' — R$ 297, buyer: pedro@email.com, status: approved, commission: R$ 89.10 (30%). 2) 'Data Science eBook' — R$ 47, buyer: lucas@email.com, approved. 3) 'Python Bootcamp' — R$ 197, buyer: carla@email.com, approved. 4) 'AI Mastery Course' — R$ 297, buyer: fernanda@email.com, approved. 5) 'Data Science eBook' — R$ 47, buyer: rafael@email.com, refunded. Active subscriptions: 89 total. Monthly: 52 (avg R$ 49/mo). Annual: 37 (avg R$ 397/yr). Next renewals this week: 8 subscriptions. Churn rate: 4.2% monthly. Would you like a detailed revenue breakdown?


## ❓ FAQ

**Q: Can I track how many students completed my course?**
Yes. Use `list_students` to see all enrolled students across your products. Then use `get_student_progress` with a Student ID to see their course completion percentage, modules accessed, and last activity date. This helps identify students at risk of dropping off.

**Q: Does Hotmart require two credentials for authentication?**
Yes. Hotmart uses OAuth 2.0 Client Credentials flow. You need a **Client ID** and a **Client Secret**, generated in the Hotmart Developer Portal. These are used to obtain a Bearer token automatically — the server handles token exchange internally.

**Q: Can I view a detailed breakdown of my sales revenue?**
Yes. Use `get_sales_summary` for aggregated data including total revenue, number of sales, and average ticket. Use `get_sales_history` for individual transactions with status, price breakdowns, commissions, and buyer information. Combine with `list_products` to correlate revenue per product.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hotmart-alternative](https://vinkius.com/mcp/hotmart-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotmart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hotmart-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotmart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotmart-alternative": {
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
