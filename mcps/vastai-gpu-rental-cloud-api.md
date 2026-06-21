# Vast.ai (GPU Rental Cloud API) MCP Server

Rent high-performance GPUs for AI and deep learning. Search marketplace offers, deploy Docker containers, and manage your cloud GPU fleet.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vastai-gpu-rental-cloud-api)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 4

## Description
Connect your **Vast.ai** account to any AI agent to orchestrate high-performance GPU rentals through natural language. Access the world's most affordable GPU marketplace directly from your workspace.

### What you can do

- **GPU Discovery** — Search the marketplace for specific hardware like RTX 4090, A100, or H100 using flexible JSON queries.
- **Instant Deployment** — Rent instances immediately by specifying an offer ID, a Docker image (like PyTorch or TensorFlow), and required disk space.
- **Fleet Management** — List all your active rented instances to monitor status, connection details, and costs.
- **Resource Optimization** — Terminate and delete instances instantly when your compute tasks are finished to save on costs.

### How it works

1. Subscribe to this server
2. Enter your Vast.ai API Key
3. Start searching for and renting GPUs from Claude, Cursor, or any MCP-compatible client

No more manual searching through web consoles. Your AI can now find the best price-to-performance GPU and deploy your environment in seconds.

### Who is this for?

- **AI Researchers** — quickly spin up powerful nodes for training or fine-tuning models without leaving the chat.
- **Data Scientists** — manage compute resources for heavy data processing tasks directly from your IDE.
- **DevOps Engineers** — automate the lifecycle of GPU-accelerated containers and monitor cloud infrastructure costs.


## Available Tools
- **delete_instance**: Delete/Terminate an instance on Vast.ai
- **list_instances**: List your rented instances on Vast.ai
- **rent_instance**: Rent a GPU instance on Vast.ai
- **search_offers**: The query should be a JSON string like {"gpu_name":{"eq":"RTX 4090"}}.

Search for available GPUs on Vast.ai


## Installation & Usage

To install and use the **Vast.ai (GPU Rental Cloud API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vastai-gpu-rental-cloud-api](https://vinkius.com/mcp/vastai-gpu-rental-cloud-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
