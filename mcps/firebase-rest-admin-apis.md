# Firebase (REST & Admin APIs) MCP Server

Manage Firebase Realtime Database, Firestore, and Auth via REST APIs — query data, manage users, and send FCM messages directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/firebase-rest-admin-apis)

## Overview
**Category:** developer-tools
**Tools Count:** 14

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


## Installation & Usage

To install and use the **Firebase (REST & Admin APIs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firebase-rest-admin-apis](https://vinkius.com/mcp/firebase-rest-admin-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
