# EyePop.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eyepopai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eyepopai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eyepopai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Add computer vision to your apps with pre-trained models for object detection, face recognition, and image classification.

## Description
Connect your **EyePop.ai** account to any AI agent and take full control of your real-time computer vision orchestration and automated visual intelligence through natural conversation.

### What you can do

- **Visual Analysis Orchestration** — List and manage your entire portfolio of visual models (Pops) programmatically, retrieving detailed detection metadata
- **Media Stream Intelligence** — Programmatically trigger and monitor real-time media stream processing to maintain a perfectly coordinated visual knowledge pipeline
- **Object Detection Architecture Monitoring** — Access real-time status updates for detected objects and track confidence scores directly through your agent
- **Metadata Management** — Programmatically retrieve bounding box coordinates and classification IDs to maintain a perfectly coordinated data record
- **Operational Monitoring** — Verify account-level API connectivity and monitor visual processing volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your EyePop.ai dashboard (Profile > API Keys)
3. Start orchestrating your visual intelligence from Claude, Cursor, or any MCP client

No more manual reviewing of video frames or missing critical object detections. Your AI acts as your dedicated visual coordinator and computer vision architect.

### Who is this for?

- **Security & Ops Managers** — instantly retrieve detection summaries and monitor visual alerts using natural language commands
- **Retail Analysts** — verify individual foot traffic metadata and track customer behavior without leaving your creative workspace
- **Developers** — integrate high-speed EyePop.ai vision data into custom monitoring and alerting tools through simple AI queries


## Available Tools
- **analyze_image**: Returns detected objects, labels, and bounding boxes.

Analyze an image
- **analyze_video**: Returns temporal object detection results.

Analyze a video
- **check_eyepop_status**: Verify EyePop API connectivity
- **create_pop**: Create a visual pipeline
- **get_account**: Get account info
- **get_model**: Get model details
- **get_pop**: Get pipeline details
- **list_detections**: List detections
- **list_models**: List available models
- **list_pops**: List all visual pipelines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EyePop.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Pops in my EyePop.ai account."

**🤖 AI Agent:**
> I've retrieved your Pops. You currently have 5 active visual pipelines, including 'Main Security Feed' and 'Store Counter A'. Would you like the detailed detection metadata for any of them?

---

**👤 You:**
> "Show the detected objects from 'Main Security Feed' for the last hour."

**🤖 AI Agent:**
> Visual intelligence orchestrated! For Main Security Feed, I've identified 10 object detections in the last hour, including 5 'Persons' and 2 'Vehicles'. I've retrieved the technical confidence metadata for your review. Need help setting an alert for specific objects?

---

**👤 You:**
> "Check the processing status for Pop ID 'pop_123'."

**🤖 AI Agent:**
> Operational monitoring orchestrated! For pop_123, the current status is 'RUNNING' and processing 30 frames per second. Your API connection is healthy. Shall I retrieve the detailed resource usage metadata for this pipeline?


## Installation & Usage

To install and use the **EyePop.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eyepopai](https://vinkius.com/mcp/eyepopai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
