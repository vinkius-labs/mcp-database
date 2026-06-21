# Deel MCP Server

Manage global contracts, team members, invoices, payments, time-off, and expenses — global HR for AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deel)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Integrate **Deel**, the all-in-one global people platform, directly into your AI workflow. Manage your international team, track contracts and compliance, monitor invoices and payments, and handle time-off requests using natural language.

### What you can do

- **Contract Management** — List and view contracts with terms, compensation, and compliance status across 150+ countries.
- **Global Team Directory** — Browse and retrieve profiles for all your employees and contractors in one unified view.
- **Payroll & Invoice Tracking** — Monitor invoices, view payment history, and track processing status for your global workforce.
- **Leave & Expense Oversight** — Monitor time-off requests and review submitted expenses with approval statuses.

### How it works

1. Connect the Deel integration to your AI assistant.
2. Authorize using your Deel API Token (found in your Developer settings).
3. Orchestrate your global HR operations through intuitive conversation.

### Who is this for?

- **HR Managers** — Quickly check contract statuses and team details on the go.
- **Finance Teams** — Monitor global payroll invoices and payment processing via chat.
- **Operations Leaders** — Track time-off and expenses across international entities effortlessly.


## Available Tools
- **list_contracts**: Returns contract metadata including legal type (e.g., fixed, PAYG, milestone), current status, and high-level compensation structures.

List all contracts
- **list_expenses**: Returns expense report metadata including receipt attachments, currency amounts, and the current review status (approved/rejected/pending).

List submitted expenses
- **get_contract**: Resolves detailed terms, compliance requirements, specific compensation rates, and effective dates.

Get contract details
- **list_people**: Returns a list of team members including their professional roles, geographical locations, and the nature of their Deel integration (employee vs. contractor).

List all people (employees and contractors)
- **get_person**: Resolves personal metadata, active and historical contract links, and cumulative payment history within the Deel platform.

Get person details
- **list_invoices**: Returns invoice metadata including billing amounts, issue dates, and current payment status (e.g., paid, pending, overdue).

List all invoices
- **list_payments**: Returns data on disbursement amounts, recipient identifiers, and the technical status of each transfer.

List all payments
- **list_time_off**: Returns a collection of time-off requests including requested dates, leave categories, and the current approval status for each entry.

List time-off requests
- **list_tasks**: Returns task descriptions, due dates, and completion status for milestone-based engagements.

List tasks for a contract
- **list_milestones**: Returns identifiers, payment amounts, and projected achievement dates for defined project stages.

List contract milestones


## Installation & Usage

To install and use the **Deel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deel](https://vinkius.com/mcp/deel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
