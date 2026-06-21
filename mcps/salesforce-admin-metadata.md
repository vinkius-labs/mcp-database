# Salesforce Admin & Metadata MCP Server

Manage users, explore object schemas, monitor org limits, search metadata, execute Apex, and audit profiles through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-admin-metadata)

## Overview
**Category:** industry-titans
**Tools Count:** 8

## Description
The **Salesforce Admin** toolkit for AI agents.

### What you can do
- **Users** — List and search active users with profiles and roles
- **Objects** — List all objects, describe schemas with field details
- **Limits** — Monitor API calls, storage, and rate limits
- **Metadata** — Search Apex classes, triggers, flows via Tooling API
- **Apex** — Execute anonymous Apex code
- **Profiles** — List security profiles

### Who is this for?
- **Admins** — Manage 20+ orgs from one conversation
- **Consultants** — Explore client orgs instantly
- **Architects** — Understand data models in seconds


## Available Tools
- **sf_describe_object**: Returns every field with: API name, label, data type (string/number/date/reference/picklist/boolean), whether required or nullable, max length, reference target objects (for lookups), and picklist values (for picklist fields). Essential for understanding the data model before creating or querying records. Use when the user asks "what fields does Account have?" or needs to know valid picklist values.

Describe the full schema of a Salesforce object — all fields, data types, relationships, picklist values, and validation rules
- **sf_execute_apex**: Returns compilation success/failure, execution result, and debug logs. Use for admin tasks (data cleanup, batch operations), testing hypotheses, or running one-off scripts. CAUTION: this executes real code on the org — can modify data. Example: System.debug('Hello World');

Execute anonymous Apex code on the Salesforce org for admin tasks, data fixes, testing, or one-off operations
- **sf_org_limits**: Returns current usage vs. maximum for: daily API calls, data storage, file storage, SOQL queries, DML operations, email invocations, and more. Flags any limits below 10% remaining. Use for capacity monitoring, API governance, or when the user asks about org health and limit consumption.

Get API and storage usage limits for the Salesforce org — current consumption vs. maximum for API calls, storage, and more
- **sf_list_objects**: Returns all objects with their API name, label, whether they are queryable, createable, and custom. Includes standard objects (Account, Contact, Lead, Opportunity, Case), custom objects (ending in __c), and managed package objects. Essential for data model discovery: "what objects are available?", "do we have a custom invoices object?"

List all queryable and createable objects in the Salesforce org — standard, custom, and managed package objects
- **sf_list_profiles**: Returns profile name, description, user type, and license type. Profiles control what users can see and do in Salesforce — they define object permissions, field-level security, and page layouts. Use when the user asks about permissions, needs to audit access levels, or wants to understand the security model.

List Salesforce profiles (permission sets) with name, description, and user type for access control auditing
- **sf_list_users**: Returns user name, email, profile name, role name, user type (Standard/Chatter/etc.), and last login date. Use when the user asks about team members, needs user IDs for record assignment, wants to audit active accounts, or check last login dates for license management.

List active Salesforce users with their profile, role, email, user type, and last login date for team management
- **sf_search_metadata**: Supported objects: ApexClass, ApexTrigger, CustomField, ValidationRule, Flow, FlowDefinition, CustomObject, etc. Example: SELECT Id, Name, Body FROM ApexClass WHERE Name LIKE '%Account%'. Use when the user asks about code, automations, custom fields, or configuration metadata in the org.

Search Salesforce metadata via the Tooling API — find Apex classes, triggers, custom fields, validation rules, flows, and more
- **sf_search_users**: Returns user name, email, username, profile, role, and login info. Use to find a specific person in the org, look up who owns a record, or get user IDs for API operations.

Search Salesforce users by name, email, or username to find specific team members or administrators


## Installation & Usage

To install and use the **Salesforce Admin & Metadata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-admin-metadata](https://vinkius.com/mcp/salesforce-admin-metadata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
