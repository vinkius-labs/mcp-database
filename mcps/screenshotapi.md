# ScreenshotAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/screenshotapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/screenshotapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/screenshotapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Capture full-page website screenshots programmatically with custom viewport sizes, delays, and rendering options via a simple API.

## Description
Connect your **ScreenshotAPI.net** account to any AI agent and take full control of your website rendering and visual orchestration through natural conversation. ScreenshotAPI provides a high-performance API for capturing pixel-perfect screenshots, generating PDFs, and simulating various devices directly from your chat interface.

### What you can do

- **Visual Orchestration** — Capture high-quality screenshots of any URL with support for lazy-loading and dynamic content programmatically.
- **Full-Page & PDF Intelligence** — Generate comprehensive full-page captures or professional PDF documents from web pages directly from the AI interface.
- **Mobile & Device Emulation** — Simulate specific devices (e.g., iPhone, Android) and viewports to monitor responsive designs via natural language.
- **Stealth & Ad-Block Control** — Automatically block ads and cookie banners to ensure clean visual results without manual intervention.
- **Operational Monitoring** — Track system health and manage rendering options like dark mode and custom CSS injection using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ScreenshotAPI.net Token from your dashboard
3. Start capturing and managing web visuals from Claude, Cursor, or any MCP-compatible client

No more manual 'Print Screen' or browser debugging. Your AI acts as a dedicated visual QA engineer or content coordinator.

### Who is this for?

- **Marketing Managers** — quickly retrieve visual snapshots of competitor campaigns without switching apps.
- **QA Engineers** — automate the capture of responsive design tests across multiple devices via natural conversation.
- **Content Creators** — streamline the generation of website previews and PDF reports directly within the chat.


## Available Tools
- **capture_clean_screenshot_no_ads**: Capture screenshot without ads or cookies
- **capture_dark_mode_screenshot**: Capture screenshot in dark mode
- **capture_delayed_screenshot**: Useful for lazy-loading elements.

Capture screenshot after a delay
- **capture_new_screenshot_no_cache**: Force a fresh screenshot bypass cache
- **capture_full_length_screenshot**: Capture the entire length of a webpage
- **capture_mobile_view_screenshot**: Capture a screenshot using a mobile viewport
- **convert_webpage_to_pdf**: Save a webpage as a PDF file
- **capture_specific_element**: Capture a screenshot of a specific CSS element
- **capture_website_screenshot**: Returns a hosted image link.

Capture a standard screenshot of a URL
- **capture_webp_format_screenshot**: Capture screenshot in WebP format
- **check_api_health**: net service.

Verify Screenshot API status
- **get_api_quota_info**: Get account API usage information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ScreenshotAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a clean mobile screenshot of the Apple homepage (https://www.apple.com) without any cookie banners or ads."

**🤖 AI Agent:**
> I've successfully captured a clean mobile viewport screenshot of the Apple homepage. All cookie consent banners and overlays were blocked. You can view the final image here: https://screenshotapi.net/storage/apple-mobile-clean.png

---

**👤 You:**
> "Capture a full-length screenshot of the Stripe pricing page (https://stripe.com/pricing) to check their new tier layout."

**🤖 AI Agent:**
> The full-page capture is complete. I scrolled from top to bottom to render the entire Stripe pricing page accurately. Here is the full-length high-resolution image: https://screenshotapi.net/storage/stripe-pricing-full.png

---

**👤 You:**
> "Generate a professional PDF export of the latest Y Combinator blog post at https://blog.ycombinator.com/yc-top-companies-2024."

**🤖 AI Agent:**
> I've converted the Y Combinator blog post into a high-quality PDF document. The formatting and typography have been preserved perfectly. You can download the PDF report here: https://screenshotapi.net/storage/yc-top-companies-2024.pdf


## Installation & Usage

To install and use the **ScreenshotAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/screenshotapi](https://vinkius.com/mcp/screenshotapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
