# Coder Legion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coder-legion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect AI agents to Coder Legion, a developer community: browse and publish posts and Q&A, jobs, content series, groups, the developer directory and community tags through the official API.

## Description
Turn any AI agent into a resident of Coder Legion, a community of thousands of developers where engineers ask and answer questions, publish articles, follow launches and dev stories, and post or browse jobs.

### What you can do

- **Publish to the post stream** — `create_post` for a new article or question, `update_post` to revise one, `add_post_comment` to join a discussion
- **Work the job board** — `list_jobs` for postings, `get_job` for full listings (description, requirements, metadata)
- **Build series** — `list_series` / `get_series` to browse, `create_series` / `update_series` to shape multi-part collections
- **Run groups** — `create_group` / `update_group` / `delete_group`, `join_group`, `add_group_member` and `list_group_members`
- **Research the community** — `list_developers` for the directory and `list_tags` / `create_tag` for the topic vocabulary

### How it works

1. Subscribe to this server
2. Generate an API key in your Coder Legion account dashboard and paste it into the credential field
3. Ask your agent to browse, publish, comment or manage content

Every route in the Coder Legion API is authenticated with that key. When the key is missing or invalid, tools return a clear error pointing at the dashboard; when a resource id does not exist, the tool says so, so the agent can recover instead of guessing. Write tools modify real community content, so they run only when you explicitly ask, and any server rejection comes back verbatim with the field names, so the agent can correct and retry. List tools support best-effort `limit`/`offset` pagination — the server's default page applies when it ignores those values.

### Who is this for?

- **Developers** — keep a running awareness of community discussions, series and new jobs, and publish your own articles and answers
- **Recruiters and founders** — scan the community job board and developer directory for signals
- **Content and DevRel teams** — track what the community writes about, publish series, and manage groups


## Available Tools (20)
- **add_post_comment**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Posts a comment on an existing Coder Legion post, using the post id returned by list_posts or get_post. Use it to answer a question, leave feedback or start a discussion. The comment is public to the community. Requires the CODERLEGION_API_KEY credential.

Add a comment to a Coder Legion post
- **create_post**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Creates and publishes a new post in the Coder Legion stream. Pass a title, and the body/content when the post carries text; tags are comma-separated topic labels. Confirm the content with the user before publishing when in doubt. Requires the CODERLEGION_API_KEY credential.

Publish a new post (article or question) to Coder Legion
- **update_post**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Replaces fields of an existing post, using the post id returned by list_posts or get_post. Pass only the fields to change (title, body, comma-separated tags). Use it to fix or improve content you or the user previously published. Requires the CODERLEGION_API_KEY credential.

Update an existing Coder Legion post by id
- **update_series**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Replaces fields of an existing series, using the series id returned by list_series or get_series. Pass only the fields to change (title, description, comma-separated tags). Requires the CODERLEGION_API_KEY credential.

Update an existing Coder Legion series by id
- **create_group**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Creates a new community group. Pass a name, and a description and comma-separated tags when relevant. The returned group record is what update_group, join_group and list_group_members work with. Requires the CODERLEGION_API_KEY credential.

Create a new community group on Coder Legion
- **create_series**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Creates a new multi-part content series in the Coder Legion collection. Pass a title, and a description and comma-separated tags when relevant. The series record returned by the server is what get_series and update_series work with. Requires the CODERLEGION_API_KEY credential.

Create a new content series on Coder Legion
- **create_tag**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Creates a new topic tag in the Coder Legion vocabulary, so future posts can be scoped to it. Pass the tag name and an optional description. Requires the CODERLEGION_API_KEY credential.

Create a new community tag on Coder Legion
- **delete_group**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Deletes an existing community group, using the group id. This is destructive: the group and its association with members are removed. Only use it when the user explicitly asks to delete a group, and confirm before acting. Requires the CODERLEGION_API_KEY credential.

Delete a Coder Legion community group by id
- **get_job**: Returns the complete listing record (description, requirements and metadata) so the agent can evaluate or report on it. Use it after list_jobs to inspect a specific role. Requires the CODERLEGION_API_KEY credential.

Get full details for a Coder Legion job posting by its id
- **get_post**: Returns the complete post record (content and associated metadata) so the agent can read, quote or summarize it. Use it when a specific post id is known; list_posts when exploring. Requires the CODERLEGION_API_KEY credential.

Get full details for a Coder Legion post by its id
- **get_series**: Returns the complete series record, including its structure and parts, so the agent can summarize the collection or navigate its content. Requires the CODERLEGION_API_KEY credential.

Get full details for a Coder Legion series by its id
- **join_group**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Joins an existing group on Coder Legion, using the group id. An optional role describes the member's part in the group. Use it when the user wants to become a member of a community group. Requires the CODERLEGION_API_KEY credential.

Join an existing Coder Legion community group
- **list_developers**: Returns a page of developer records. Use it to find or research developers in the community. The public, keyless version of this directory is available without credentials through the Coder Legion Developers connection. limit and offset are best-effort pagination. Requires the CODERLEGION_API_KEY credential.

List the Coder Legion developer directory
- **list_group_members**: Returns member records. Use it after create_group or join_group to see who is in the group. limit and offset are best-effort pagination. Requires the CODERLEGION_API_KEY credential.

List the members of a Coder Legion community group
- **list_jobs**: Returns a page of job records (title, employer and metadata). Use it when the user asks about work available in the community. Open a specific listing with get_job using the returned id. limit and offset are best-effort pagination. Requires the CODERLEGION_API_KEY credential.

List job postings on the Coder Legion job board
- **list_posts**: Returns a page of post records with their title, id and basic metadata. Use it to discover recent or featured community content, or as the first step before opening a specific post with get_post. limit and offset are best-effort pagination — if the server ignores them, its default page is returned. Requires the CODERLEGION_API_KEY credential.

List Coder Legion posts — the community articles and Q&A threads
- **list_series**: Returns a page of series records (title, author and metadata). Use it to discover structured, follow-up-able content, or as a first step before opening a specific series with get_series. limit and offset are best-effort pagination. Requires the CODERLEGION_API_KEY credential.

List content series on Coder Legion (multi-part post collections)
- **list_tags**: Returns tag records. Use it to learn which topics the community covers, or to pick a tag to scope content before browsing posts. limit and offset are best-effort pagination. Requires the CODERLEGION_API_KEY credential.

List community tags on Coder Legion
- **update_group**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Replaces fields of an existing group, using the group id returned by create_group. Pass the new name and/or description. Requires the CODERLEGION_API_KEY credential.

Update an existing Coder Legion group by id
- **add_group_member**: Returns the server's response record when it succeeds. Field names follow the API's public contract; if the server rejects the payload, the error comes back verbatim so the field names or values can be corrected. Adds a developer to a community group, using the group id. Pass the developer to add (user id) and an optional role. Use it after create_group or join_group to grow a group's roster. Requires the CODERLEGION_API_KEY credential.

Add a member to a Coder Legion community group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coder Legion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest posts on Coder Legion and tell me what the community is discussing."

**🤖 AI Agent:**
> I listed the most recent Coder Legion posts. The stream is dominated by engineering articles (TypeScript type guards, boot protocols, AI tracking) and Q&A threads; here are the 10 newest with titles, authors and categories. Want me to open any of them in full?

---

**👤 You:**
> "Show me the open jobs on the Coder Legion job board and summarize what each role is about."

**🤖 AI Agent:**
> I pulled the current Coder Legion job listings and summarized each: titles, companies, remote/onsite and the main requirements. The full description of any listing can be fetched on demand. Which one should I open in detail?

---

**👤 You:**
> "What topics does the Coder Legion community use tags for, and who are some active developers in the directory?"

**🤖 AI Agent:**
> I listed the community tags and a page of developer profiles. The tags span TypeScript, Python, AI tooling, DevOps and more; the directory page includes names, taglines and verified badges. I can open any post, series or developer record you point at.


## ❓ FAQ

**Q: Do I need a Coder Legion account and API key?**
Yes. Coder Legion API calls are authenticated with an account API key. Create an account at coderlegion.com, generate a key from your account dashboard, and paste it into the credential field. Without a valid key every tool returns a clear 401 error pointing at the fix.

**Q: What can this connection do?**
Reading: the post stream (articles and Q&A threads), the job board, content series, groups, the developer directory and the community tag vocabulary. Writing: publish, update and comment on posts, create and update series, create, update and delete groups, join a group, add group members, list group members, and create new tags. Twenty tools in total; the write tools only run when you explicitly ask.

**Q: How do I get an API key?**
Log in to coderlegion.com, open the API docs section (coderlegion.com/api-docs) and generate a key for your account. The key is tied to your account and is the only credential this server needs.

**Q: What happens if the API rate-limits me or an id does not exist?**
The engine turns API failures into actionable errors: a rate limit tells you to wait and retry, an unknown id tells you to check the id (use the matching list tool to find valid ones), and an invalid key tells you to regenerate it in the dashboard. No silent failures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coder-legion](https://vinkius.com/en/ai-agent-connect/coder-legion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coder Legion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coder-legion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coder Legion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coder-legion": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
