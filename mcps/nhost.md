# Nhost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nhost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Nhost authentication and storage — handle user sign-ins, registrations, profile management, and file uploads directly from any AI agent.

## Description
Connect your **Nhost** project to any AI agent to manage your backend services through natural language. This server provides a comprehensive interface for Nhost's Authentication and Storage services.

### What you can do

- **Authentication Flows** — Sign in users via email/password, OTP, magic links, or anonymous sessions using `signin_email_password`, `signin_otp_email`, and `signin_passwordless_email`.
- **User Management** — Register new accounts with `signup_email_password`, retrieve profiles with `get_user`, and handle password resets or email changes.
- **Session Control** — Refresh access tokens and securely sign out users from single or all devices using `refresh_token` and `signout`.
- **Cloud Storage** — Upload files directly to your Nhost buckets using the `upload_file` tool, supporting both text and base64 content.

### How it works

1. Subscribe to this server
2. Provide your Nhost Auth and Storage URLs from your project dashboard
3. Start managing users and files from Claude, Cursor, or any MCP client

### Who is this for?

- **Full-stack Developers** — manage user sessions and test auth flows directly from the IDE without switching to the browser.
- **DevOps Engineers** — automate user provisioning and file management tasks through simple conversation.
- **Support Teams** — quickly verify user profile information and account status to resolve customer issues faster.


## Available Tools (15)
- **get_file**: Supports optional image transformation parameters.

Download the complete file content
- **get_user**: Requires NHOST_JWT credential.

Retrieve the authenticated user profile information
- **refresh_token**: Generate a new JWT access token using a valid refresh token
- **reset_password**: Request a password reset email
- **signin_anonymous**: Create an anonymous user session
- **signin_email_password**: Authenticate a user with email and password
- **signin_otp_email**: Initiate email-based one-time password authentication
- **signin_passwordless_email**: Initiate passwordless authentication by sending a magic link
- **signout**: Invalidate refresh tokens and end the session
- **signup_email_password**: Register a new user account
- **signup_otp_email**: Register a new user account using email OTP
- **upload_file**: Returns metadata for the processed file.

Upload a file to a bucket
- **change_email**: Requires elevated NHOST_JWT credential.

Request to change the authenticated user email
- **delete_file**: Permanently delete a file
- **get_file_presigned_url**: Retrieve a presigned URL for a file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nhost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sign in user dev@example.com with password 'securePass123'."

**🤖 AI Agent:**
> I've initiated the sign-in process for dev@example.com using `signin_email_password`. The session has been successfully established.

---

**👤 You:**
> "Show me the profile details for the current authenticated user."

**🤖 AI Agent:**
> Fetching profile... Using `get_user`, I've retrieved the account details: User ID 'usr_7721', Email 'dev@example.com', and the account is currently active.

---

**👤 You:**
> "Upload a file named 'config.json' with content '{"theme": "dark"}'."

**🤖 AI Agent:**
> Processing upload... I've used `upload_file` to save 'config.json' to your Nhost Storage. The file is now available in your default bucket.


## ❓ FAQ

**Q: How can I retrieve the profile of the currently logged-in user?**
Use the `get_user` tool. It fetches the authenticated user's profile information, including their ID and metadata, provided a valid JWT is configured.

**Q: Is it possible to store documents or images using this server?**
Yes. The `upload_file` action allows you to send raw text or base64 content along with a filename directly to your Nhost Storage bucket.

**Q: Can I initiate a login without requiring a password?**
Absolutely. Use the `signin_passwordless_email` tool to send a magic link to a user's email address for a seamless passwordless authentication experience.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nhost](https://vinkius.com/mcp/nhost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nhost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nhost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nhost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nhost": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
