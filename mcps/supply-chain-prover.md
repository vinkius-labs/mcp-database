# Supply Chain Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supply-chain-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/supply-chain-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/supply-chain-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [operations](../categories/operations.md)

A manufacturer asked an AI to plan seasonal inventory. The AI said 'maintain adequate stock levels.' No forecast model. No EOQ. No safety stock. No supplier diversification. No bullwhip mitigation. Ordered on gut feel from a single Shenzhen supplier, shipped by air because 'urgent,' and watched demand amplify through three echelons until the warehouse held 340% of actual demand. This tool forces five axes: demand forecasting, inventory optimization, supplier risk diversification, logistics cost-per-unit analysis, and bullwhip effect mitigation.

## Description
## The Problem

LLMs commit five supply chain failures:
1. **Gut-Feel Forecasting** — qualitative guesses instead of statistical models with MAPE.
2. **Inventory Blindness** — 'enough stock' instead of EOQ, safety stock, carrying cost math.
3. **Single-Source Naivety** — one supplier in one country = catastrophic risk.
4. **Logistics Handwaving** — 'we ship it' instead of mode selection, cost/kg, last-mile analysis.
5. **Bullwhip Ignorance** — demand amplification 2-5x at each echelon ignored.

### The 5 Supply Chain Axes

| Axis | Pivot | Formula / Rule |
|---|---|---|
| **Demand** | Statistical | Model + CI + MAPE. Not 'we expect growth.' |
| **Inventory** | Modeled | EOQ = √(2DS/H). Safety stock = Z×σ×√L. |
| **Suppliers** | Diversified | Top supplier <30% spend. Dual-sourced. |
| **Logistics** | Optimized | $/kg per mode. Last-mile = 40-53% of total. |
| **Bullwhip** | Mitigated | POS sharing. Batch reduction. Lead time compression. |


## Available Tools
- **validate_supply_chain**: Before any supply chain decision, call this tool: (1) DEMAND FORECAST — statistical model (exponential smoothing, ARIMA, Holt-Winters). Data period (minimum 24 months). Confidence interval (95% CI). MAPE (target < 15%). "We expect growth" is NOT a forecast — a forecast has a model, data, and error metric, (2) INVENTORY — EOQ formula: √(2DS/H) for every SKU. Safety stock: Z × σ × √L (service level, demand variability, lead time). Reorder point: average demand during lead time + safety stock. Carrying cost: 18-25% of inventory value/year (storage, insurance, depreciation, obsolescence), (3) SUPPLIER RISK — concentration % per supplier (max 30% of any critical category). Lead time coefficient of variation (CV < 0.2 = reliable). Geographic spread (min 2 regions). Dual-source plan for all components with lead time > 2 weeks. Financial health of top 3 suppliers, (4) LOGISTICS — mode selection: air ($4-6/kg), sea ($0.20-0.50/kg), road ($0.30-0.80/kg), rail ($0.15-0.30/kg). Cost per unit shipped. Last-mile as % of total cost (typically 40-55%). Warehouse network: number, location, coverage radius. Hub-and-spoke vs direct, (5) BULLWHIP — POS data sharing with supply chain tiers. Order batch frequency (smaller = better). Price stabilization (eliminate bulk discount incentives). Lead time compression targets. VMI (Vendor Managed Inventory) where applicable. If rejected, your supply chain has a single point of failure.

Structured reflection tool for Toyota-level supply chain reasoning — forces systematic analysis of demand forecasting, inventory optimization, supplier risk, logistics efficiency, and bullwhip mitigation. Based on Toyota Production System (Taiichi Ohno), Just-in-Time philosophy, and lessons from global supply chain disruptions (2020-2024). Catches Gut-Feel Forecasting (no statistical model behind demand predictions — a bicycle manufacturer: "We expect demand to grow 20% next year based on market trends." No model. No confidence interval. No historical MAPE analysis. Reality: they ordered 20% more aluminum frames. Actual demand grew 3%. Result: 8,500 unsold frames at $120 each = $1.02M in dead inventory. Warehouse carrying cost: 25% of inventory value/year = $255K/year in storage, insurance, depreciation. A competitor used exponential smoothing (α=0.3) on 36 months of historical sales data. Forecast: +7% ± 4% (95% CI). MAPE: 8.2%. Ordered +11% (upper bound). Result: sold 100% of inventory. Zero dead stock. Rule: "we expect" is not a forecast. A forecast has: model name, data period, confidence interval, and MAPE < 15% to be actionable), Inventory Blindness (no EOQ/safety stock calculation — guessing purchase quantities — a restaurant chain orders napkins "when we run low." Annual demand: 500,000 napkins. Cost per napkin: $0.03. Ordering cost: $45/order (delivery minimum). Carrying cost: 20% of value/year. EOQ = √(2 × 500,000 × $45 / ($0.03 × 0.20)) = √(45,000,000 / 0.006) = 86,603 napkins per order. Optimal: 5.8 orders/year (every 9 weeks). Current: ordering 20,000 at a time = 25 orders/year. Excess ordering cost: 19.2 extra orders × $45 = $864/year — on NAPKINS alone. Apply this blindness across 200 SKUs: $47K/year in unnecessary ordering costs. Safety stock: σ = 12,000/month, lead time = 2 weeks. Z(95%) × σ × √L = 1.65 × 12,000 × √0.5 = 13,991 napkins. Without safety stock: 3 stockouts per year. Each stockout = emergency order at 2.5x premium. Fix: calculate EOQ and safety stock for EVERY SKU. The math exists since 1913 — use it), Single-Source Naivety (all eggs in one basket — supplier concentration risk — an electronics assembler: 100% of their capacitors from one factory in Shenzhen. "They have the best price." March 2021: factory fire. Production halted for 6 weeks. The assembler: zero alternative suppliers. Zero safety stock (JIT philosophy misapplied). Production line idle for 6 weeks. Revenue lost: $4.2M. Customers switched to competitor. Recovery took 9 months — 3 customers never returned ($1.8M/year recurring revenue lost permanently). Ford Motor Company 2021: semiconductor shortage from concentrated Asian supply = $3.5B lost revenue. Toyota — the SAME company that invented JIT — maintains 2-4 week semiconductor buffers AND dual-source critical components. Toyota lost $1.1B vs Ford's $3.5B in the same crisis. Rule: no single supplier > 30% of any critical category. Dual-source all components with lead time > 2 weeks. Geographic diversification: do not source 100% from one region), Logistics Handwaving (no cost-per-unit or mode-selection analysis — a clothing brand ships everything by air freight. "Speed is our advantage." Air freight: $4.20/kg. Average garment: 0.5kg. Shipping cost: $2.10/unit. Garment wholesale price: $12. Shipping = 17.5% of revenue. Alternative: sea freight for basic inventory (90-day lead time styles). Sea freight: $0.35/kg. Shipping cost: $0.18/unit. Shipping = 1.5% of revenue. For trend-sensitive items (10% of catalog): air freight justified ($2.10/unit on $25 retail). For basics (90% of catalog): sea freight saves $1.92/unit × 200,000 units = $384,000/year. Last-mile delivery: $4.50/package average. This is 53% of total logistics cost. Optimization: regional fulfillment centers (3 hubs instead of 1 central warehouse). Last-mile cost reduction: $4.50 → $2.80/package = $340,000/year saved on 200,000 shipments. Total logistics savings: $724,000/year. No one "analyzed" it because "we just ship things"), and Bullwhip Ignorance (demand amplification across supply chain echelons — P&G's beer game (MIT Sloan experiment): a 10% increase in retail demand becomes 20% at the distributor, 40% at the manufacturer, 80% at the raw material supplier. Why: each echelon adds safety margin to the order. Retailer orders 110% (10% buffer). Distributor orders 125% (15% buffer on the already-inflated signal). Manufacturer orders 150%. Supplier orders 200%. When retail demand normalizes: supplier has 2x inventory. Write-down. Layoffs. This happened globally in 2021-2022: pandemic demand spike → massive overordering → 2023 inventory glut (Amazon, Target, Walmart wrote down billions in excess inventory). Fix: share POS (point-of-sale) data directly with all supply chain tiers — the supplier sees ACTUAL demand, not the amplified signal. Reduce order batching: smaller, more frequent orders (daily vs monthly). Stabilize pricing: eliminate bulk discount incentives that encourage overordering. Compress lead times: shorter lead time = less forecasting error = less safety stock = less bullwhip). Call once per supply chain decision, procurement strategy, or logistics optimization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supply Chain Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We expect demand to grow next quarter. We keep enough stock from our trusted supplier. Logistics handles shipping. Orders follow demand."

**🤖 AI Agent:**
> GUT_FEEL_FORECAST — Five failures: no statistical model, no inventory math, single supplier, logistics handwaving, bullwhip amplification.

---

**👤 You:**
> "Demand: exponential smoothing (α=0.3) on 24 months, forecast 12,400 ± 1,800 units/month (95% CI), MAPE 11.2%. Inventory: EOQ 1,467 units, safety stock 1,005, reorder point 6,797, carrying 24.8%. Suppliers: 3 suppliers — 38% Vietnam, 35% India, 27% Mexico. Lead time CV 0.22. Logistics: 60% sea ($0.18/kg), 30% road ($1.20/kg), 10% air urgent, cost/unit $2.34, last-mile 47%. Bullwhip: daily POS EDI to top-3 suppliers, weekly orders (not monthly), EDLP reduced forward-buying 35%, lead time compressed 45→28 days."

**🤖 AI Agent:**
> SUPPLY_CHAIN_PROVEN — All five axes validated at Toyota level.

---

**👤 You:**
> "Demand: ARIMA(1,1,1) on 36 months, 8,200 units/month ± 900 (95% CI), MAPE 8.7%. Inventory: EOQ 982 units, safety stock 645, reorder 4,120, carrying 21.3%. Suppliers: 2 suppliers — 72% Guangdong, 28% Guangdong (same region). Lead time CV 0.41. Logistics: 85% sea, 15% air, cost/unit $1.90. Bullwhip: monthly order batches."

**🤖 AI Agent:**
> SINGLE_SOURCE_NAIVE — Forecast and inventory pass. Suppliers FAIL: 100% in Guangdong = catastrophic geographic concentration. Lead time CV 0.41 = unreliable. Diversify to at least 2 regions. Then fix monthly batching (bullwhip amplification).


## Installation & Usage

To install and use the **Supply Chain Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supply-chain-prover](https://vinkius.com/mcp/supply-chain-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
