# Vast.ai (GPU Rental Cloud API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vastai-gpu-rental-cloud-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vastai-gpu-rental-cloud-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vastai-gpu-rental-cloud-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Rent high-performance GPUs for AI and deep learning. Search marketplace offers, deploy Docker containers, and manage your cloud GPU fleet.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vast.ai (GPU Rental Cloud API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for available RTX 4090 GPU offers on Vast.ai."

**🤖 AI Agent:**
> I've found several RTX 4090 offers. The cheapest is Offer ID 728391 at $0.42/hr with 24GB VRAM. Would you like to see more details or rent this one?

---

**👤 You:**
> "Rent offer 728391 using the 'pytorch/pytorch' image and 50GB of disk."

**🤖 AI Agent:**
> Success! I have initiated the rental for Offer ID 728391. Your new Instance ID is 1029384. It is currently spinning up with the PyTorch image.

---

**👤 You:**
> "List all my current active instances on Vast.ai."

**🤖 AI Agent:**
> You have one active instance (ID: 1029384) running an RTX 4090. Status: 'running', IP: 123.45.67.89, Cost: $0.42/hr.


## Installation & Usage

To install and use the **Vast.ai (GPU Rental Cloud API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vastai-gpu-rental-cloud-api](https://vinkius.com/mcp/vastai-gpu-rental-cloud-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
