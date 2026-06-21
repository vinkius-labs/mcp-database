# Farcaster (Decentralized Social Protocol) MCP Server

Interact with the Farcaster protocol — manage channels, moderate casts, and explore social graphs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/farcaster-decentralized-social-protocol)

## Overview
**Category:** communication-messaging
**Tools Count:** 22

## Description
Connect your **Farcaster** account to any AI agent and take full control of your decentralized social interactions through natural conversation.

### What you can do

- **Channel Management** — List all Farcaster channels, fetch specific channel details, and manage your follows/unfollows directly.
- **Advanced Moderation** — Hide or unhide casts, pin important content to channels, and manage user bans to maintain community standards.
- **Social Graph Exploration** — Query followers of any channel or see which channels a specific user (FID) is following.
- **User Relations** — Manage blocked users and inspect social connections within the protocol.
- **Protocol Identity** — Access account verifications and primary addresses associated with Farcaster IDs.

### How it works

1. Subscribe to this server
2. Enter your Farcaster Auth Token (from Warpcast or your developer portal)
3. Start managing your social presence from Claude, Cursor, or any MCP-compatible client

No more switching between apps to moderate your channel or check your social growth. Your AI acts as a dedicated community manager and protocol explorer.

### Who is this for?

- **Community Managers** — instantly moderate casts, pin announcements, and manage channel members without leaving your workflow.
- **Web3 Developers** — query channel data and user verifications directly from your code editor.
- **Social Power Users** — automate how you follow channels and track social graphs across the Farcaster ecosystem.


## Available Tools
- **ban_channel_user**: Requires authentication.

Ban a user from a channel
- **block_user**: Requires authentication.

Block a user
- **create_signed_key_request**: Create a signed key request
- **follow_channel**: Requires authentication.

Follow a Farcaster channel
- **get_channel**: Get a single Farcaster channel
- **get_current_fname_by_fid**: Get current fname of an FID
- **get_current_fname_owner**: Get current owner of an fname
- **get_primary_address**: Get a user primary wallet address
- **get_signed_key_request**: Get signed key request status
- **list_account_verifications**: List account verifications for a user
- **list_all_channels**: List all Farcaster channels
- **list_blocked_users**: Get blocked users
- **list_channel_followers**: List followers of a Farcaster channel
- **list_creator_rewards**: Get weekly top creator rewards
- **list_developer_rewards**: Get weekly top developer rewards
- **list_fname_transfers**: Can be filtered by name, fid, or timestamp.

Get fname transfer history
- **list_moderated_casts**: List moderation actions in a channel
- **list_user_following_channels**: List channels a user follows
- **moderate_cast**: Requires authentication and moderator privileges.

Hide or unhide a cast in a channel
- **pin_cast**: Requires authentication.

Pin a cast to a channel
- **register_or_transfer_fname**: Requires EIP-712 signature from the FID custody address.

Register or transfer an fname
- **unfollow_channel**: Requires authentication.

Unfollow a Farcaster channel


## Installation & Usage

To install and use the **Farcaster (Decentralized Social Protocol)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/farcaster-decentralized-social-protocol](https://vinkius.com/mcp/farcaster-decentralized-social-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
