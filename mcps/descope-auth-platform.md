# Descope (Auth Platform) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/descope-auth-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage user authentication flows via Descope — initiate OTPs, Magic Links, Enchanted Links, and OAuth directly from your AI agent.

## Description
Connect **Descope** to your AI agent to manage and test user authentication flows through natural conversation. Descope is a drag-and-drop authentication and user management platform for any application.

### What you can do

- **OTP Authentication** — Initiate and verify One-Time Passwords via Email, SMS, or Voice using tools like `auth_otp_signup_email` and `auth_otp_verify_email`.
- **Magic & Enchanted Links** — Send secure sign-up/sign-in links and poll for session completion with `auth_magiclink_signup_email` or `auth_enchantedlink_poll`.
- **OAuth Integration** — Start OAuth flows with providers like Google and exchange codes for active sessions using `auth_oauth_authorize`.
- **Password Management** — Handle traditional password-based sign-ups via `auth_password_signup`.
- **Session Verification** — Verify tokens and manage the authentication lifecycle directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Descope Project ID and optional Management Key
3. Start managing your auth flows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Test authentication logic and verify OTP/Magic Link flows without leaving the terminal or IDE.
- **QA Engineers** — Automate the verification of sign-up and sign-in processes through natural language queries.
- **Product Managers** — Quickly inspect how different auth providers and methods are configured in your project.


## Available Tools (33)
- **mgmt_create_access_key**: Create a new access key (M2M)
- **mgmt_create_permission**: Create a new permission
- **mgmt_create_role**: Create a new role
- **mgmt_create_tenant**: Create a new tenant
- **mgmt_create_user**: Create a new user
- **mgmt_delete_user**: Delete a user
- **auth_enchantedlink_poll**: Poll for Enchanted Link session
- **auth_enchantedlink_signup**: Sign up a user via Enchanted Link
- **auth_enchantedlink_verify**: Verify an Enchanted Link token
- **auth_exchange_access_key**: Exchange an access key for a session JWT
- **auth_get_keys**: Get public keys for session validation
- **mgmt_get_user**: Load a user by login ID
- **mgmt_list_tenants**: Load all tenants
- **auth_magiclink_signup_email**: Sign up or sign in a user via Magic Link
- **auth_magiclink_verify**: Verify a Magic Link token
- **auth_oauth_authorize**: Start OAuth flow
- **auth_oauth_exchange**: Exchange OAuth code for session
- **auth_otp_signin_email**: Sign in a user via Email OTP
- **auth_otp_signup_email**: Sign up a user via Email OTP
- **auth_otp_signup_sms**: Sign up a user via SMS OTP
- **auth_otp_signup_voice**: Sign up a user via Voice OTP
- **auth_otp_verify_email**: Verify an Email OTP
- **auth_otp_verify_sms**: Verify an SMS OTP
- **auth_otp_verify_voice**: Verify a Voice OTP
- **auth_password_reset**: Reset a user password
- **auth_password_signin**: Sign in a user with a password
- **auth_password_signup**: Sign up a user with a password
- **mgmt_search_users**: Search for users
- **mgmt_update_user**: Update an existing user
- **auth_webauthn_signin_finish**: Finish WebAuthn sign in
- **auth_webauthn_signin_start**: Start WebAuthn sign in
- **auth_webauthn_signup_finish**: Finish WebAuthn sign up
- **auth_webauthn_signup_start**: Start WebAuthn sign up


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Descope (Auth Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sign up a new user with email dev-test@example.com using OTP."

**🤖 AI Agent:**
> I've initiated the signup process for dev-test@example.com using `auth_otp_signup_email`. An OTP code has been sent to that address. Please provide the code to complete verification.

---

**👤 You:**
> "Verify the OTP code 998877 for user dev-test@example.com."

**🤖 AI Agent:**
> Verifying code 998877 via `auth_otp_verify_email`... Success! The user is now authenticated and a session has been created.

---

**👤 You:**
> "Start a Google OAuth flow with redirect URL https://example.com/callback."

**🤖 AI Agent:**
> I've triggered `auth_oauth_authorize` for Google. You can now proceed with the authentication at the provided redirect URL.


## ❓ FAQ

**Q: How do I verify an email OTP code sent to a user?**
Use the `auth_otp_verify_email` tool by providing the user's `loginId` (email) and the `code` they received. The agent will return the session details if the verification is successful.

**Q: Can I start a Google OAuth login flow using this server?**
Yes. Use the `auth_oauth_authorize` tool with 'google' as the `provider` and specify your `redirectURL`. The agent will initiate the OAuth flow for you.

**Q: What is the purpose of the enchanted link polling tool?**
The `auth_enchantedlink_poll` tool allows the agent to check the status of a pending enchanted link authentication using a `pendingRef`. It helps determine if the user has clicked the link and completed the session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/descope-auth-platform](https://vinkius.com/mcp/descope-auth-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Descope (Auth Platform)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `descope-auth-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Descope (Auth Platform)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "descope-auth-platform": {
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
