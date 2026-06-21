# DummyJSON MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dummyjson)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dummyjson-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dummyjson-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access a comprehensive suite of dummy data for testing and prototyping — products, carts, and user authentication directly from your AI agent.

## Description
Connect to **DummyJSON** to simulate real-world API interactions within your AI environment. Perfect for developers needing instant access to structured data for building, testing, and demonstrating applications without setting up a backend.

### What you can do

- **Product Catalog** — List, search, and filter products by category or ID using `list_products` and `search_products` to test e-commerce flows.
- **Cart Management** — Simulate shopping cart operations including listing, retrieving, and creating user carts with `list_carts` and `add_cart`.
- **Authentication Simulation** — Test login flows, profile retrieval, and token refreshing using simulated JWT endpoints like `auth_login` and `auth_get_me`.
- **Data Mutation** — Perform simulated additions, updates, and deletions of products via `add_product`, `update_product`, and `delete_product` to verify UI/UX logic.

### How it works

1. Subscribe to this server
2. (Optional) Provide a DummyJSON token if required by your specific implementation
3. Start querying and manipulating dummy data from Claude, Cursor, or any MCP client.

### Who is this for?

- **Frontend Developers** — quickly mock data for UI components without waiting for backend readiness.
- **QA Engineers** — test edge cases and API response handling with predictable dummy data.
- **AI Researchers** — provide agents with a safe sandbox environment to practice tool-calling and data manipulation.


## Available Tools
- **add_cart**: Create a new cart
- **add_comment**: Add a comment
- **add_post**: Add a post
- **add_product**: Add a new product (simulated)
- **add_recipe**: Add a recipe
- **add_todo**: Add a todo
- **add_user**: Add a user
- **delete_cart**: Delete a cart
- **delete_comment**: Delete a comment
- **delete_post**: Delete a post
- **delete_product**: Delete a product (simulated)
- **delete_recipe**: Delete a recipe
- **delete_todo**: Delete a todo
- **delete_user**: Delete a user
- **filter_users**: Filter users by key and value
- **get_cart**: Get a single cart by ID
- **get_comment**: Get a single comment by ID
- **get_comments_by_post**: Get comments for a specific post
- **auth_get_me**: Retrieve the profile of the currently authenticated user
- **get_post_comments**: Get comments for a post
- **get_post**: Get a single post by ID
- **get_posts_by_user**: Get posts by user
- **get_product**: Get a single product by ID
- **get_products_by_category**: Get products by category
- **get_quote**: Get a single quote by ID
- **get_random_quote**: Get a random quote
- **get_random_quotes**: Get multiple random quotes (max 10)
- **get_random_todo**: Get a random todo
- **get_recipe**: Get a single recipe by ID
- **get_recipes_by_meal_type**: Get recipes by meal type
- **get_recipes_by_tag**: Get recipes by tag
- **get_todo**: Get a single todo by ID
- **get_user_carts**: Get carts belonging to a specific user
- **get_user_posts**: Get posts by user
- **get_user_todos**: Get todos by user
- **get_user**: Get a single user by ID
- **list_carts**: Get all carts
- **list_categories**: Get all category objects
- **list_category_list**: Get all category names
- **list_comments**: Get all comments
- **list_post_tags**: Get all post tags
- **list_posts**: Get all posts
- **list_products**: Get all products
- **list_quotes**: Get all quotes
- **list_recipe_tags**: Get all recipe tags
- **list_recipes**: Get all recipes
- **list_todos**: Get all todos
- **list_users**: Get all users
- **auth_login**: Authenticate a user and receive JWT tokens
- **auth_refresh_token**: Extend the session using a refresh token
- **search_posts**: Search posts
- **search_products**: Search products
- **search_recipes**: Search recipes
- **search_users**: Search users
- **update_cart**: Update cart items
- **update_comment**: Update a comment
- **update_post**: Update a post
- **update_product**: Update a product (simulated)
- **update_recipe**: Update a recipe
- **update_todo**: Update a todo
- **update_user**: Update a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DummyJSON** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all products in the 'smartphones' category."

**🤖 AI Agent:**
> I've retrieved the products for you. In the 'smartphones' category, I found items like the iPhone 9, iPhone X, and Samsung Universe 9. Would you like the details for any of these?

---

**👤 You:**
> "Search for 'laptop' and limit the results to 3."

**🤖 AI Agent:**
> Searching... I found 3 laptops for you: MacBook Pro, Samsung Galaxy Book, and Microsoft Surface Laptop 4. Which one should we look at first?

---

**👤 You:**
> "Simulate a login for user 'emilys' with password 'emilyspass'."

**🤖 AI Agent:**
> Login successful! I've authenticated as 'emilys'. I now have the JWT access token and refresh token for this session. What would you like to do next?


## Installation & Usage

To install and use the **DummyJSON** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dummyjson](https://vinkius.com/mcp/dummyjson)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
