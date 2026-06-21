# Mabl (AI-Powered Test Automation) MCP Server

Manage E2E testing via Mabl — trigger test plans, monitor execution results, and perform AI-driven failure analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mabl-ai-powered-test-automation)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Mabl** account to any AI agent and take full control of your AI-powered E2E testing and quality orchestration through natural conversation.

### What you can do

- **Plan Orchestration** — List all test plans and trigger immediate executions across specific environments (staging, production) directly from your agent
- **Execution Monitoring** — Track the real-time status of ongoing test runs and retrieve detailed outcome summaries including pass/fail rates and durations
- **AI Failure Analysis** — Deep-dive into execution results to extract precise failure reasons, diagnostic insights, and visual screenshots for rapid debugging
- **Environment Audit** — List configured testing environments and retrieve associated variables to ensure accurate test execution context
- **App & API Discovery** — Enumerate all monitored applications and their target URLs (web + API) to manage your testing grid securely
- **Label & Tag Management** — Discover and list plan labels used to group and trigger specific testing suites across your organization

### How it works

1. Subscribe to this server
2. Enter your Mabl API Key
3. Start managing your test automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Automation Engineers** — trigger complex test plans and analyze failure diagnostics through natural conversation without leaving your IDE
- **Software Developers** — verify build quality and retrieve session screenshots to debug UI regressions directly from your workspace
- **DevOps Teams** — audit CI/CD test results and monitor environment health across multiple Mabl projects efficiently


## Available Tools
- **mb.list_apps**: Use this to lookup application details.

List all applications on Mabl. Mabl is an AI-powered E2E testing platform for web, mobile, and API testing with self-healing tests
- **mb.get_app**: Get full details of a Mabl application including name, description, targets (web URLs + API base URLs), and labels
- **mb.list_envs**: ). Returns env names, IDs, and environment variables.

List all environments on Mabl
- **mb.list_plans**: Returns plan names, statuses, triggers, and linked apps/envs.

List all test plans (run policies) on Mabl
- **mb.trigger_plan**: Trigger a Mabl plan run via deployment event
- **mb.list_executions**: List latest execution results on Mabl
- **mb.get_execution**: Get full details of a Mabl execution result including status, duration, test outcomes, failure analysis, and screenshots
- **mb.list_tests**: List all API tests on Mabl
- **mb.list_labels**: Returns label names and associated plan counts.

List all labels (tags) used in Mabl plans
- **mb.workspace_info**: Does not require args.

Get workspace info for the authenticated Mabl API key including workspace name, org, and key metadata


## Installation & Usage

To install and use the **Mabl (AI-Powered Test Automation)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mabl-ai-powered-test-automation](https://vinkius.com/mcp/mabl-ai-powered-test-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
