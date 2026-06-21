# Nash Game Theory Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nash-game-theory-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [strategy](../categories/strategy.md)

Every strategy proposed by an AI treats the world as a single-player game. No opponents. No counter-moves. No equilibrium analysis. The AI said 'our competitive advantage' without mapping a single opponent's payoff, analyzing their best response, or checking if the strategy survives rational counter-play. Nash proved in 1950 that every finite game has at least one equilibrium — ignoring this is not a strategic choice, it is a mathematical error. This tool forces five game-theoretic axes: payoff mapping, equilibrium analysis, information structure, mechanism design, and repeated dynamics.

## Description
## The Problem

LLMs commit five game-theoretic failures:
1. **Single-Player Delusion** — reasons as if alone in the universe.
2. **Equilibrium Blindness** — strategies that any rational opponent can exploit.
3. **Information Naivety** — assumes complete information when games are incomplete.
4. **Mechanism Passivity** — plays the game instead of designing it.
5. **One-Shot Fallacy** — ignores that repeated games produce cooperation.

### The 5 Nash Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Payoff** | Mapped | Every player, every action, every payoff combination. |
| **Equilibrium** | Found | Nash Equilibrium: no unilateral deviation improves any player. |
| **Information** | Analyzed | Complete vs incomplete. Hidden info. Bayesian reasoning. |
| **Mechanism** | Designed | Change the rules. The master designs the game. |
| **Dynamics** | Modeled | Repeated games. Reputation. Tit-for-tat. Credible commitment. |

### Verdict Matrix

```
Axis 1 fails → SINGLE_PLAYER_DELUSION
Axis 2 fails → EQUILIBRIUM_BLIND
Axis 3 fails → INFORMATION_NAIVE
Axis 4 fails → MECHANISM_PASSIVE
Axis 5 fails → ONE_SHOT_FALLACY
All pass     → EQUILIBRIUM_PROVEN
```


## Available Tools
- **validate_nash_game_theory**: Think like John Nash: (1) PAYOFF MAPPING — name EVERY player, their available actions, and ALL payoff combinations. Draw the matrix. "Our strategy" without "their best response" is a wish, not strategy, (2) EQUILIBRIUM ANALYSIS — find the Nash Equilibrium. Does your chosen strategy survive every opponent playing their BEST RESPONSE? If any player can improve by deviating alone, the strategy is exploitable, (3) INFORMATION STRUCTURE — complete or incomplete information? What does each player know and not know? Who is signaling? Who is bluffing? Bayesian updating: what do they BELIEVE about your beliefs? (4) MECHANISM DESIGN — can you REDESIGN the game? Change the rules, add commitments, alter incentive structures, introduce information revelation mechanisms? The master does not play the game — the master designs it, (5) REPEATED DYNAMICS — is this a one-shot or repeated interaction? Reputation effects, tit-for-tat, credible commitment, discount factor. NPV of cooperation vs. one-shot defection gain. If rejected, fix the specific game-theoretic reasoning gap.

Structured reflection tool for game-theoretic strategic reasoning — forces payoff matrix construction, Nash Equilibrium identification, information structure analysis, mechanism design evaluation, and repeated game dynamics modeling before any competitive or multi-player strategic decision. The most demanding prover for any LLM — game theory requires holding multiple agents' simultaneous reasoning in a consistent strategic framework. Catches Single-Player Delusion (optimizing your strategy without modeling opponents' best responses — a SaaS company prices at $49/month to maximize signups. Analysis considers only: price elasticity of demand, CAC payback, and margin target. Never modeled: Competitor A's best response is to undercut at $39/month (they have lower COGS). Competitor B's best response is to bundle their product into an existing suite at +$0/month. After both responses: the $49 price point generates 60% less volume than projected. Every pricing decision is a game — your "optimal price" assumes opponents stand still), Equilibrium Blind (choosing a strategy that is exploitable via unilateral deviation — a Nash Equilibrium is a strategy profile where NO player can improve their payoff by changing their strategy alone. A startup offers a "matching discount" policy: "we will match any competitor's price." Sounds defensive. But this is NOT an equilibrium — the competitor's best response is to publicly list a $1 price for a single day, force the match, then revert. The matching policy has no equilibrium because it incentivizes predatory pricing probes. If your strategy changes when one opponent deviates, it is not stable), Information Naive (assuming all players have the same information — in a hiring negotiation: the employer knows the budget range ($120K-$160K), the internal equity bands, and how urgently the role needs filling. The candidate knows their BATNA (competing offer), their minimum acceptable salary, and their assessment of the employer's urgency. Neither knows the other's private information. The candidate signals high value by being slow to respond. The employer signals abundance by mentioning "many candidates." Both are bluffing — but Bayesian reasoning (updating beliefs from signals) determines the negotiated outcome. Perfect information games are textbook exercises — real decisions involve hidden information, signaling, and belief updating), Mechanism Passive (accepting the game as given instead of redesigning the rules — "the master does not play the game — the master designs it." A procurement team runs a standard sealed-bid auction. They receive 3 bids. The lowest bid is suspiciously low (45% below estimate). Second lowest is 12% below. They are stuck: accept the suspicious bid (risk of cost overruns, change orders), or reject it (justify to stakeholders). Mechanism redesign: switch to a Vickrey auction (second-price sealed bid). Bidders truthfully reveal their costs because the winning bidder pays the second-lowest price. No incentive to underbid. No suspicious outliers. The game rules were the problem, not the players), and One-Shot Fallacy (treating a repeated interaction as a single encounter — a freelancer can overcharge a first-time client by 40% and they might not know. One-shot game: overcharging is the dominant strategy (higher payoff, no consequence). Repeated game: the client discovers market rates, leaves a bad review, tells 5 colleagues. NPV of cooperation: $5,000/year × 10 years × referrals = $150,000 lifetime value. NPV of one-shot defection: $2,000 extra once. Discount factor δ = 0.95 — cooperation is the dominant strategy when δ > (defection gain / cooperation stream). Reputation effects, tit-for-tat, and credible commitment mechanisms transform the equilibrium from defection to cooperation in repeated games). Call once per competitive strategy, negotiation, pricing decision, or multi-player interaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nash Game Theory Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our strategy is to dominate the market. We will outperform competitors with our unique position. The market will respond predictably under existing rules. Maximize this deal for short-term gain."

**🤖 AI Agent:**
> SINGLE_PLAYER_DELUSION — Five failures: no opponent mapping, unstable strategy, naive assumptions, passive mechanism, one-shot thinking.

---

**👤 You:**
> "Players: Us (enter/wait), Incumbent (accommodate/price-war). Payoffs: (enter,accommodate)=(8,5), (enter,war)=(-3,2), (wait,any)=(0,10). NE: (enter,accommodate) — stable, no unilateral deviation improves either. Info: incomplete — cost structure hidden, signal via pricing. Bayesian: accommodate → P(high-cost)=0.7. Mechanism: price-match guarantee changes best response. Repeated: quarterly for 5yr, δ=0.9, NPV cooperation $2M vs defection $400K."

**🤖 AI Agent:**
> EQUILIBRIUM_PROVEN — Game-theoretic strategy validated. All five axes pass. Execute.

---

**👤 You:**
> "Two competitors are in a pricing standoff. We charge $49/mo, they charge $45/mo. If we drop to $39, they will likely match. Market has 10K potential customers, currently split 55/45 in our favor. Switching costs are low."

**🤖 AI Agent:**
> Classic Prisoner Dilemma with price war dynamics. NE analysis: (drop, match) = both lose margin with no share gain. Mechanism design needed — differentiate on value, not price. Add switching costs through long-term commitments. Convert to repeated game: multi-year contracts with loyalty pricing break the one-shot race to the bottom.


## ❓ FAQ

**Q: Why is single-player thinking a mathematical error?**
Nash (1950): every finite game with n players has at least one equilibrium. If your strategy does not account for every other player's best response, it is not in equilibrium — any rational opponent can exploit it. 'Our competitive advantage' without mapping the opponent's counter-move is a wish, not a proof.

**Q: What does 'design the game' mean?**
Mechanism design (Myerson, 2007 Nobel): instead of playing the game as given, change the rules, incentive structure, or information revelation so the DESIRED equilibrium becomes dominant. Add contracts, commitments, auctions, or public information that makes cooperation rational and defection costly.

**Q: Why do repeated games change everything?**
Axelrod (1984): in repeated Prisoner's Dilemma, tit-for-tat — cooperate first, then mirror opponent's last move — wins. Cooperation emerges when: (1) interaction repeats, (2) reputation has value, (3) discount factor is high enough. One-shot defection gains $X. Repeated cooperation gains NPV of $10X. Reputation is the mechanism.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nash-game-theory-prover](https://vinkius.com/mcp/nash-game-theory-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nash Game Theory Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nash-game-theory-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nash Game Theory Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nash-game-theory-prover": {
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
