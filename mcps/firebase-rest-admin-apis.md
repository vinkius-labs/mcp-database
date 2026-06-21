# Firebase (REST & Admin APIs) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firebase-rest-admin-apis)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/firebase-rest-admin-apis-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/firebase-rest-admin-apis-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Firebase Realtime Database, Firestore, and Auth via REST APIs — query data, manage users, and send FCM messages directly from your AI agent.

## Description
Connect your **Firebase** project to any AI agent to manage your backend infrastructure through natural language. This server leverages Firebase REST APIs to provide direct access to Realtime Database, Cloud Firestore, and Authentication services.

### What you can do

- **Realtime Database** — Perform GET, PUT, PUSH, PATCH, and DELETE operations on your JSON data trees at any path.
- **Cloud Firestore** — List collections, retrieve specific documents, and manage records with full CRUD support.
- **Authentication** — Sign up new users, authenticate existing ones with email/password, and look up profile data using ID tokens.
- **Cloud Messaging** — Send FCM notifications to specific devices or topics directly from the conversation.

### How it works

1. Subscribe to this server
2. Enter your Firebase Project ID and Web API Key
3. Start querying your database or managing users from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — Quickly inspect database state, patch records, or test Auth flows without leaving your code editor.
- **DevOps Engineers** — Automate data maintenance tasks and verify user credentials during troubleshooting sessions.
- **Product Managers** — Query live data for quick status checks or user verification without needing a custom admin dashboard.


## Available Tools
- **auth_lookup**: Get user data from Firebase Auth
- **auth_sign_in**: Sign in a user with email and password
- **auth_sign_up**: Sign up a new user or sign in anonymously
- **fcm_send_message**: Send a message via Firebase Cloud Messaging
- **firestore_create_doc**: If documentId is omitted, Firestore generates one.

Create a new document in Cloud Firestore
- **firestore_delete_doc**: Delete a document from Cloud Firestore
- **firestore_get_doc**: Get a single document from Cloud Firestore
- **firestore_list_docs**: List documents in a Cloud Firestore collection
- **firestore_patch_doc**: Update or insert a document in Cloud Firestore
- **rtdb_delete**: Delete data from Firebase Realtime Database
- **rtdb_get**: Read data from Firebase Realtime Database
- **rtdb_patch**: Update specific children in Firebase Realtime Database
- **rtdb_push**: Push data to Firebase Realtime Database (appends)
- **rtdb_put**: Write data to Firebase Realtime Database (overwrites)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Firebase (REST & Admin APIs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the data at path 'configs/app_settings' from the Realtime Database."

**🤖 AI Agent:**
> I've retrieved the settings from 'configs/app_settings'. The current configuration includes `maintenance_mode: false`, `min_version: '2.1.0'`, and `theme: 'dark'`. Would you like to update any of these values?

---

**👤 You:**
> "List all documents in the 'products' collection in Firestore."

**🤖 AI Agent:**
> I found 3 documents in the 'products' collection: 'laptop_pro_15', 'wireless_mouse_x', and 'usb_c_hub'. Would you like to see the full details for any of these products?

---

**👤 You:**
> "Sign up a new user with email 'dev-test@example.com' and password 'SecretPass123'."

**🤖 AI Agent:**
> The user has been successfully created. The new UID is `abc123xyz`. I've also received an ID token for this session. Should I look up the profile details for this new account?


## Installation & Usage

To install and use the **Firebase (REST & Admin APIs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firebase-rest-admin-apis](https://vinkius.com/mcp/firebase-rest-admin-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
