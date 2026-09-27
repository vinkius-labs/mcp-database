# Paris Trees & Street Amenities MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-trees-street-amenities)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Keyless Paris outdoor data: the city tree inventory, public drinking fountains, heat-island cooling spaces & activities, public AED defibrillators and water shops — filter by arrondissement and type.

## Description
The City of Paris's outdoor-environment inventories — trees, water, heat-island response and AEDs — keyless, from opendata.paris.fr.

### What you can do
- **find_trees** — the city tree inventory: species (French label + scientific name), trunk diameter, planting year, ownership and location; filter by arrondissement, domaniality, genus or species
- **tree_species_ranking** — the tree species ranked by count across the inventory
- **find_drinking_fountains** — the public drinking fountains, with type, availability and location (filter by object type, commune and availability)
- **find_cooling_shelters** — the green spaces identified as cooling refuges against heat islands, with opening status and 24h availability
- **find_cooling_activities** — the outdoor sites and activities run for heat-island response, with type, fee and arrondissement
- **find_defibrillators** — the public AED defibrillators, by establishment type, postal code and installation state
- **find_water_shops** — the small shops selling "eau de Paris" (refill points), by shop name and street

### Who is this for
Anyone planning outside time in Paris: a walk with shade (trees + fountains), a heat-wave plan (cooling shelters and activities), or a public-health question (where is the nearest AED, where can I refill water). Text filters are exact matches on stored values — use the ranking tool to discover species values first. Page with limit (max 100) and offset.


## Available Tools (7)
- **find_water_shops**: Use it to answer "where can I buy bottled water / refills". The source data stores names and streets in uppercase (some with source typos), and the postal code column is a placeholder ("0") — filter on the street (voie, exact stored value such as "AVENUE DAUMESNIL") or the shop name (name, exact stored value) instead. Page with limit/offset (100 rows max per call).

Find Paris water shops ("eau de Paris")
- **find_cooling_activities**: Use it to answer "where can I take shelter / cool off indoors". Filters are exact stored values: type is "Lieux de culte", "Ombrière pérenne", "Piscine", "Musée", "Bibliothèque", "Brumisateur" or "Bains-douches"; payant is "Non"/"Oui"; arrondissement is "75001".."75020". Page with limit/offset (100 rows max per call).

Find heat-island cooling sites and activities
- **find_cooling_shelters**: Use it to answer "where can I cool off in summer / during a heat wave". Filters are exact stored values: type is "Bois", "Promenades ouvertes", "Cimetières", "Jardinets décoratifs" or similar; arrondissement is "75001".."75020"; ouvert_24h is "Oui"/"Non"; canicule_ouverture is "Oui" (heat-wave opening) or "Non"; statut_ouverture is "Ouvert". Page with limit/offset (100 rows max per call).

Find heat-island cooling green spaces
- **find_defibrillators**: Use it to answer "is there a defibrillator near …". Filters are exact stored values: type_etabl is "Gymnase", "Eglise", "Bibliothèque", "Piscine", "Mairie d'arrondissement", "Musée", "Parcs et jardins", "Conservatoire" or similar; code_post is the 5-digit postal code, "75001".."75020"; etat_inst is "Existant". Page with limit/offset (100 rows max per call).

Find public AED defibrillators in Paris
- **find_drinking_fountains**: Use it to answer "where can I drink water". Filters are exact stored values: type_objet is "FONTAINE_BOIS" (the bulk of the network), "FONTNE_WALLACE" (historic wallace fountains), "BORNE_FONTAINE", "FONTAINE_ARCEAU" or "FTNE_PETILLANTE" (fizzy); commune is "PARIS 1ER ARRONDISSEMENT" .. "PARIS 20EME ARRONDISSEMENT" or a suburb such as "BAGNEUX", "PANTIN", "IVRY-SUR-SEINE"; dispo is "OUI" (available) or "NON" (out of order). Page with limit/offset (100 rows max per call).

Find public drinking fountains in Paris
- **find_trees**: ). Use it to answer "how many / which chestnuts on the Champs-Élysées", "remarkable trees", "trees near me by street". Filters are exact stored values: arrondissement is "PARIS 1ER ARRDT" .. "PARIS 20E ARRDT", "BOIS DE BOULOGNE", "BOIS DE VINCENNES" or a suburb such as "HAUTS-DE-SEINE"; domanialite is "Alignement", "Jardin", "CIMETIERE", "DASCO", "PERIPHERIQUE", "DJS", "DFPE" or "DAC"; genre is the scientific genus ("Aesculus" = chestnut, "Acer" = maple); espece is the scientific species word ("hippocastanum"); libellefrancais is the common French name ("Marronnier"); remarquable is "OUI" (the ~180 remarkable trees) or "NON". Page with limit/offset (100 rows max per call).

Search the Paris tree inventory
- **tree_species_ranking**: The facet parameter selects the classification level: "libellefrancais" (common French name, e.g. "Marronnier"), "genre" (scientific genus, e.g. "Aesculus"), "espece" (scientific species word), "domanialite" (where the trees stand) or "stadedeveloppement" (growth stage). Use it before find_trees to pick the exact filter values and to see what a street or park is dominated by.

Rank tree species in the Paris inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Trees & Street Amenities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many plane trees does the city have, and which species dominate?"

**🤖 AI Agent:**
> tree_species_ranking returns the species ranked by count (pass the top value to rank the most common); find_trees with espece set to the species label then pages the individual trees, with diameter, planting year and location.

---

**👤 You:**
> "Where can I get drinking water or refill my bottle near the Louvre?"

**🤖 AI Agent:**
> find_drinking_fountains (filter by commune or availability, e.g. dispo: "oui") lists the public fountains with their locations; find_water_shops lists the small shops selling "eau de Paris" by street (voie) or shop name — combine both to cover the louvre quarter.

---

**👤 You:**
> "Which green spaces in the 12th open 24h in summer?"

**🤖 AI Agent:**
> find_cooling_shelters with arrondissement: "12" and ouvert_24h: "oui" returns the green refuges in that arrondissement available around the clock; add canicule_ouverture to keep only the ones opened for the heat-wave plan.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: How big is the tree inventory?**
It is the full planted-tree inventory of the City of Paris (streets, squares, parks and green spaces). find_trees pages it (100 rows per call) and tree_species_ranking summarises the species mix without fetching rows.

**Q: Can I use it during a heat wave?**
Yes — find_cooling_shelters lists the green spaces designated as heat refuges (with 24h availability and opening state, incl. canicule_ouverture) and find_cooling_activities lists the outdoor cooling sites and activities, both filterable by arrondissement.

**Q: How do I find the nearest AED?**
find_defibrillators lists the public AED installations: filter by type_etabl (establishment type), code_post (postal code, e.g. "75001") or etat_inst (installation state); each row carries the location description.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-trees-street-amenities](https://vinkius.com/en/ai-agent-connect/paris-trees-street-amenities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Trees & Street Amenities** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-trees-street-amenities` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Trees & Street Amenities** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-trees-street-amenities": {
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
