# US Forest Service Trails MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/us-forest-service-trails)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

The trail inventory of the US National Forests — search trails by name, list the trails crossing any area, and read each trail's permitted uses, surface, grade and accessibility.

## Description
Connects an AI agent to the United States Forest Service's published National Trail inventory — the national record of trails on National Forest System land, every segment of it, kept in the agency's own database.

### What you can do

- **Search by name** — find trails called anything, or pin down the trail number a forest prints on its map
- **List an area** — every trail segment crossing a bounding box or a radius around a point, optionally restricted to trails managed for one mode
- **Read one trail** — surface, grade, tread width, development class, accessibility and the permitted uses for hiking, horses, bicycles, each e-bike class, motorcycles, ATVs, snowmobiles, skis and watercraft
- **Profile an area** — how many trails and how many miles, split by kind, development class and surface, without listing them

### Why it matters

The Forest Service records, for every segment, which travel modes it manages the trail for and the season each allowance runs — and it distinguishes a trail managed for a use from one that merely accepts it. That distinction is the difference between a route a forest maintains for mountain bikes and a wilderness trail where a bike happens not to be prohibited, and it is what makes an answer usable for planning rather than merely plausible.

Two properties of the source shape every answer. A trail is stored as the chain of segments sharing its number, so one trail number can return several rows, sometimes with different allowances along its length. And the layer holds National Forest System trails only: trails inside National Parks, on Bureau of Land Management land or on other agencies' ground are not in it, and an empty result inside a park boundary means exactly that.


## Available Tools (5)
- **find_trails_in_area**: Give a bounding box as bbox "west,south,east,north" — for example "-119.3,37.4,-119.1,37.6" (longitudes are negative west of Greenwich, and west must be less than east) — or a latitude, longitude and radius_km, in which case a box is built around the point. radius_km defaults to 20 and caps at 200. A use filter keeps only segments managed for that mode: hiker_pedestrian, bicycle, e_bike_class1, e_bike_class2, e_bike_class3, pack_saddle, motorcycle, atv, fourwd, snowmobile, snowcoach_snowcat, snowshoe, xcountry_ski, motor_watercraft, nonmotor_watercraft. "Managed for" is stronger than "allowed": a bicycle-managed trail is one the forest looks after for cycling. Absent a use filter, wilderness and motorized trails are listed side by side, so for a planning question name the mode. Results are paginated and sorted longest first; the response says how many match in all. An empty result inside a National Park is expected — this layer is National Forest land only.

List the National Forest trail segments that cross an area — every trail the Forest Service holds in a bounding box or around a point, optionally filtered to trails managed for one travel mode
- **get_trail_details**: Identify the trail by its trail number or by the objectid a listing returned; a number is what a forest publishes on its maps and signs. Several segments can share a number, and all of them come back, with the end-to-end length. Permitted uses are reported per segment because allowances can change along a trail — the bicycle-managed lower half and the wilderness upper half of one numbered trail are a real pattern. Geometry is included as a GeoJSON line unless include_geometry is false, which keeps the response small when only the attributes matter.

The full record of one National Forest trail — surface, grade, tread width, accessibility, permitted uses, and the surveyed line of the trail itself
- **summarize_trails_in_area**: Accepts the same area inputs as find_trails_in_area: bbox "west,south,east,north", or latitude, longitude and radius_km. Development class runs 1, primitive, to 5, fully developed, and is the quickest read of how built a trail is — a class 1 trail is a route on the ground, a class 5 is a constructed path. Use this first to size an area up, then find_trails_in_area to see the trails.

A profile of the National Forest trails in an area — how many segments, how many miles, and how they split between kinds, development classes and surfaces, without listing them
- **get_trail_uses**: The forest records each mode separately, so the answer distinguishes a trail managed for a use from one that merely accepts it, and reports the season the allowance runs — a "06/15-10/31" window means the mode is a summer allowance, and "01/01-12/31" means year-round. Absent modes are genuinely absent, not missing data. Restrictions and discouragement are flagged when the forest set them. A trail can show different allowances per segment, which is why the response groups by segment. The record here is the national inventory; a local Motor Vehicle Use Map or a seasonal closure order can still narrow it, so confirm before driving somewhere on it.

Which travel modes are allowed on one National Forest trail — hiking, horses, bicycles, each e-bike class, motorcycles, ATVs, snowmobiles, skis and watercraft — with the season each allowance runs for
- **search_trails_by_name**: Matching is case-insensitive and looks for the term anywhere in the name, so a fragment is enough: "RAINBOW" finds "Rainbow Creek" and "Rainbow Connector". The answer is segments, not trails — one trail number can cover several segments, and that is why a number can appear more than once. Each row carries the trail number to hand to get_trail_details. This inventory covers National Forest System trails only; trails in National Parks and on other agencies' land are not in it.

Find United States National Forest trails by name — search every trail in the Forest Service national inventory and return the matching trail segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Forest Service Trails** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm staying near Pasadena and want to mountain bike this weekend. What trails are there in the Angeles National Forest around me, and which ones are actually meant for bikes?"

**🤖 AI Agent:**
> I'll take a box around the Angeles National Forest north of Pasadena and keep only the trails the Forest Service manages for bicycles — that's the stronger filter than "bikes allowed", so what comes back is trail built and maintained for riding.

---

**👤 You:**
> "We're planning a backpacking trip in the Sierra National Forest near Huntington Lake. How much trail is actually there, and what's it like — wilderness singletrack or graded road?"

**🤖 AI Agent:**
> Let me profile the area first — that gives segment and mile counts split by development class and surface, which tells you whether you're looking at primitive routes or built trail, before we list anything.

---

**👤 You:**
> "Is trail 24E20 open to e-bikes and horses? I'd also like to know how steep it is and whether it's accessible."

**🤖 AI Agent:**
> I'll pull the full record for trail 24E20 — surface, grade, tread width and accessibility, plus the per-mode allowances, which the Forest Service records per segment because a trail's allowances can change along its length.


## ❓ FAQ

**Q: Does this cover trails in National Parks like Yosemite or Yellowstone?**
No. This is the Forest Service's own inventory of trails on National Forest System land, and the National Park Service keeps its trails separately. A search inside a National Park boundary returning nothing is the expected result, not a fault — the same area outside the park, on National Forest land, will return its trails. State parks and Bureau of Land Management land are also outside this layer.

**Q: Why does one trail number come back as several rows?**
The source stores a trail as the chain of segments that share its trail number, and each segment carries its own surface, grade and permitted uses. A trail can legitimately read as bicycle-managed on its lower half and closed to bikes where it enters a wilderness area further up. get_trail_details and get_trail_uses report the allowances per segment for this reason, and add the segments up into an end-to-end length.

**Q: What is the difference between a trail managed for a use and one that accepts it?**
The Forest Service keeps two columns per travel mode. A managed trail is one the agency builds and maintains for that mode — the trail is designed for it. An accepted use is tolerated on a trail managed for something else. Both are permissions, and both are reported here with the basis named, but managed is the stronger statement. Filtering an area search by a use keeps only managed trails, which is why a trail you know bikes are allowed on may not appear there.

**Q: Can I rely on this for motorized access — ATVs, motorcycles, snowmobiles?**
As a starting point, not a ruling. This is the national inventory, and the local authority is the forest's Motor Vehicle Use Map plus any seasonal closure or fire order in force on the day. The seasonal windows recorded here are real — a trail managed for motorcycles from 06/15 to 10/31 is genuinely closed to them outside that window — but a local order can narrow things further. Confirm with the forest before driving to a trailhead.

**Q: Do I need an API key or an account?**
No. The Forest Service publishes this layer openly, and the server reads it without authentication. There is no key to obtain, no quota to manage and no sign-up step.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/us-forest-service-trails](https://vinkius.com/en/ai-agent-connect/us-forest-service-trails)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Forest Service Trails** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-forest-service-trails` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Forest Service Trails** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-forest-service-trails": {
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
