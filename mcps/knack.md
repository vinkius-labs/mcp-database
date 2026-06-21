# Knack MCP Server

Manage your Knack database — list objects, query records, and perform CRUD operations via natural language.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/knack)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Knack** application to any AI agent and take full control of your no-code database through natural conversation.

### What you can do

- **Database Schema Discovery** — List all objects and fields to understand your data structure without leaving the chat
- **Record Management** — Create, retrieve, update, and delete records in any object securely
- **Advanced Querying** — Search for specific records using complex filters based on any field criteria
- **Data Auditing** — Get detailed summaries of specific records to verify information or track changes
- **Bulk Operations** — Effortlessly manage multiple records by providing structured data to your agent

### How it works

1. Subscribe to this server
2. Enter your Knack Application ID and REST API Key
3. Start managing your data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — quickly query and update business data without navigating complex dashboards
- **No-Code Developers** — verify data structures and test API interactions through natural language
- **Data Analysts** — extract specific datasets for rapid analysis and reporting


## Available Tools
- **list_objects**: This is the first step to understand the database structure and find the "Object Key" needed for record operations.

List all objects in the Knack application
- **get_object_schema**: Returns metadata including the object name, key, and high-level structure. Use this to verify you are working with the correct database table.

Get the schema of a specific Knack object
- **list_records**: You must provide the object_key. Use this to browse the actual data stored in your database.

List records for a specific Knack object
- **get_record**: Requires both the object_key and the record_id. Use this for detailed auditing of a specific entry.

Get a specific record by ID
- **create_record**: You must provide the data as a JSON string where keys are the field keys (e.g., field_1). Ensure you have checked the object schema first to know which fields are required.

Create a new record in a Knack object
- **update_record**: Provide only the fields you wish to change in the JSON string data. This is a partial update.

Update an existing record in a Knack object
- **delete_record**: Use with caution as this action cannot be undone.

Delete a record from a Knack object
- **list_object_fields**: This is crucial for understanding the data types and identifying the field keys (field_1, field_2, etc.) needed for creating or updating records.

List all fields for a specific Knack object
- **search_records**: The filters must be provided as a JSON string following the Knack Filter format (e.g., "[{\"field\":\"field_1\", \"operator\":\"is\", \"value\":\"test\"}]").

Search for records using filters
- **list_account_applications**: Use this to verify access or discover application IDs.

List all applications in the account


## Installation & Usage

To install and use the **Knack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knack](https://vinkius.com/mcp/knack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
