# Google Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Query GA4 analytics data via Google Analytics API — run reports, check realtime data, analyze funnels, and export audiences directly from any AI agent.

## Description
Connect your **Google Analytics 4 (GA4)** account to any AI agent and take full control of web and app analytics through natural conversation.

### What you can do

- **Custom Reports** — Run reports with any combination of metrics (activeUsers, screenPageViews, sessions, eventCount) and dimensions (city, country, deviceCategory, channel grouping)
- **Realtime Data** — Monitor what's happening on your site right now with live user counts, events, and traffic sources from the last 30-60 minutes
- **Batch Reports** — Execute multiple report configurations in a single API call for efficient dashboard loading
- **Metadata Discovery** — List all available metrics and dimensions for your property, including custom definitions
- **Compatibility Checks** — Validate metric/dimension combinations before running reports to avoid errors
- **Audience Exports** — List and monitor audience export jobs for user segmentation and activation
- **User Activity** — Retrieve event history for specific users for journey analysis and support investigations
- **Funnel Analysis** — Visualize user progression through conversion steps and identify drop-off points

### How it works

1. Subscribe to this server
2. Enter your Google Analytics API key from Google Cloud Console
3. Start querying analytics data, monitoring realtime metrics, and running funnel analysis from Claude, Cursor, or any MCP-compatible client

No more navigating the GA4 dashboard for every report. Your AI acts as a dedicated analytics analyst.

### Who is this for?

- **Marketing Teams** — instantly pull custom reports by channel, geography, or device without opening the GA4 interface
- **Product Managers** — monitor funnel conversion rates and identify where users drop off in signup or checkout flows
- **Data Analysts** — batch export data for further analysis in BI tools, or validate metric compatibility before complex queries
- **Support Teams** — lookup user activity by userId to investigate specific customer journeys and troubleshoot issues


## Available Tools (12)
- **batch_run_reports**: Provide property_id and an array of report configurations. Each report can have different metrics, 
dimensions, and date ranges. This is efficient for dashboard loading or comparative analysis.
The reports parameter should be a JSON array of report objects with metrics, dimensions, and dateRanges.

Run multiple reports in a single API call
- **check_compatibility**: Before running complex reports, use this to ensure compatibility between your chosen metrics and dimensions.
This prevents errors and wasted API calls. Provide property_id and the metrics/dimensions you plan to use.
Returns compatibility status and any conflicts that would prevent the report from running successfully.

Check if metrics and dimensions can be combined in a report
- **get_audience_export**: Audience exports allow you to extract user lists matching specific audience criteria.
Use this to monitor the progress of audience extraction jobs.
Provide property_id and the audience_export_id from list_audience_exports.

Get status of a specific audience export
- **get_metadata**: This includes both standard and custom metrics/dimensions with their descriptions, types, and compatibility information.
Use this to discover what data is available before building reports. The propertyId is required and can be found in your GA4 admin settings.

Get available metrics and dimensions for a GA4 property
- **get_property**: Use the property_id obtained from list_properties to inspect property configuration.

Get detailed information about a specific GA4 property
- **get_user_activity**: This shows all interactions a user has had with your property, including pageviews, events, and conversions.
Use this for user-level analysis, journey mapping, or support investigations.
The userId must match the one sent with your tracking events.

Get activity history for a specific user
- **list_accounts**: This is the top-level container for properties. Each account can contain multiple properties.
Use this to discover what accounts are available before drilling down into properties.

List all Google Analytics accounts accessible to the user
- **list_audience_exports**: Audience exports are used to extract user lists matching specific audience criteria for activation in other platforms.
Shows status (CREATING, ACTIVE, FAILED) and configuration of each export job.

List all audience export jobs for a property
- **list_properties**: Properties represent individual websites, apps, or measurement streams. 
Each property has a unique ID needed for running reports. 
Use this to find the correct property_id for report queries.

List all GA4 properties in an account
- **run_funnel_report**: This helps identify where users drop off in conversion paths like checkout flows or signup processes.
Provide property_id and a funnelSpec object defining the steps and breakdown settings.
The funnelSpec should be a JSON object with steps array containing stepName, filterExpression, and optional breakdown settings.

Run a funnel analysis report
- **run_realtime_report**: Unlike standard reports, this shows what's happening on your site/app right now.
Provide property_id and the metrics/dimensions you want to monitor in realtime.
Common realtime metrics: activeUsers, eventCount, screenPageViews.
Common realtime dimensions: city, country, deviceCategory, streamId.

Get realtime analytics data (last 30-60 minutes)
- **run_report**: You must provide the property_id, metrics (e.g., 'activeUsers', 'screenPageViews', 'eventCount'), 
and dimensions (e.g., 'city', 'pageTitle', 'sessionDefaultChannelGrouping').
Date ranges use YYYY-MM-DD format. Optional filter expression can narrow results.
Common metrics: activeUsers, screenPageViews, sessions, eventCount, engagementRate, averageSessionDuration.
Common dimensions: city, country, deviceCategory, sessionDefaultChannelGrouping, pageTitle, pagePath.

Run a custom Google Analytics report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the number of active users and pageviews by country for the last 7 days for property 123456789."

**🤖 AI Agent:**
> I've run the report for the last 7 days. Top countries by active users: United States — 45,230 active users, 189,450 pageviews; United Kingdom — 12,890 active users, 52,340 pageviews; Germany — 8,560 active users, 34,120 pageviews; Brazil — 6,780 active users, 28,900 pageviews; India — 5,420 active users, 21,560 pageviews. Total: 156,420 active users across 645,890 pageviews. Would you like a breakdown by device category or traffic source?

---

**👤 You:**
> "What's happening on the site right now? Show me realtime users by traffic source."

**🤖 AI Agent:**
> Realtime data (last 30 minutes): 847 active users right now. Top traffic sources: Organic Search — 412 users; Direct — 198 users; Social — 124 users; Paid Search — 78 users; Email — 35 users. Top pages being viewed: Homepage (/) — 234 users; Product page (/products/xyz) — 156 users; Checkout (/checkout) — 89 users. Engagement rate is 68% with average session duration of 2m 34s.

---

**👤 You:**
> "Run a funnel analysis for our checkout flow: step 1 = viewed product, step 2 = added to cart, step 3 = started checkout, step 4 = completed purchase. Show me where users drop off."

**🤖 AI Agent:**
> I've analyzed your checkout funnel. Here's the conversion flow:

1. **Viewed Product** — 12,450 users entered
2. **Added to Cart** — 4,980 users (40.0% conversion from step 1)
3. **Started Checkout** — 2,340 users (47.0% conversion from step 2)
4. **Completed Purchase** — 1,560 users (66.7% conversion from step 3)

**Overall funnel conversion rate: 12.5%** (1,560 out of 12,450)

**Biggest drop-off**: Between 'Viewed Product' and 'Added to Cart' — 60% of users leave here. This suggests product pages may need clearer CTAs, better pricing visibility, or faster load times.


## ❓ FAQ

**Q: How do I get a Google Analytics API key and what type of credentials do I need?**
You need an API Key from Google Cloud Console. Go to **console.cloud.google.com** → Select or create a project → Enable the **Google Analytics Data API v1** → Navigate to **APIs & Services > Credentials** → Click **Create Credentials > API Key**. Copy the key (starts with `AIzaSy...`). Then, in Google Analytics Admin, add the service account email with Viewer or Analyst role to your GA4 property. Paste the API key below.

**Q: What metrics and dimensions are available in GA4 and how do I find them?**
Use the `get_metadata` tool with your property_id to list all available metrics and dimensions. Common metrics include: `activeUsers`, `screenPageViews`, `sessions`, `eventCount`, `engagementRate`, `averageSessionDuration`, `conversions`. Common dimensions include: `city`, `country`, `deviceCategory`, `sessionDefaultChannelGrouping`, `pageTitle`, `pagePath`, `streamName`. The metadata response shows descriptions, types, and whether each field is a metric or dimension.

**Q: Can I get realtime data and how far back does it go?**
Yes! Use the `run_realtime_report` tool to get data from the last 30-60 minutes. Realtime reports show active users, events, and traffic sources as they happen on your site. This is useful for monitoring campaign launches, tracking live events, or checking if tracking is working correctly. Unlike standard reports which can take 24-48 hours to process, realtime data is available within minutes.

**Q: How do I analyze funnel conversion rates and identify drop-off points?**
Use the `run_funnel_report` tool with a funnel_spec JSON object defining your conversion steps. Each step includes a stepName, filterExpression (e.g., eventName equals 'page_view'), and optional breakdown settings. The response shows how many users entered each step, how many completed it, and where the biggest drop-offs occurred. This helps identify friction points in checkout flows, signup processes, or any multi-step user journey.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-analytics](https://vinkius.com/mcp/google-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-analytics": {
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
