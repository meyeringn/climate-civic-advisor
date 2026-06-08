# 🌿 Climate Civic Action Advisor

**A conversational civic tech tool connecting Philadelphia residents to climate resources, advocacy pathways, and community organizations — powered by AI.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Tool-brightgreen)](https://meyeringn.github.io/climate-civic-advisor)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Made for Philly](https://img.shields.io/badge/Made%20for-Philadelphia%20🧡🖤-blue)](https://www.phila.gov)

-----

## What It Does

Philadelphia residents face compounding climate burdens — urban heat islands, stormwater flooding, poor air quality, tree canopy gaps — that fall disproportionately on low-income neighborhoods and Disabled communities. But navigating the city’s network of programs, commissions, and advocacy organizations is genuinely hard.

The **Climate Civic Action Advisor** lets any resident describe a climate concern in plain language and receive:

- A plain-language explanation of the climate issue they’re experiencing
- 3–5 specific Philadelphia organizations, city programs, or commissions to engage with
- 2–3 concrete next steps they can take this week
- Accessibility considerations baked into every recommendation
- Random Philadelphia civic trivia to keep it human

It works like a knowledgeable neighbor — not a bureaucrat.

-----

## Why This Exists

This tool sits at the intersection of three principles:

1. **Climate equity is a disability justice issue.** Extreme heat, flooding, and air quality crises hit Disabled people and chronically ill residents hardest. Resources and action pathways must be accessible by design.
1. **Civic participation requires on-ramps.** The barrier to engagement isn’t apathy — it’s opacity. This tool lowers that barrier.
1. **AI should serve communities, not extract from them.** Every suggestion in this tool points outward — to real local organizations, real city programs, real humans doing the work.

-----

## Tech Stack

|Layer     |Tool                                                       |
|----------|-----------------------------------------------------------|
|Frontend  |React (via CDN, no build step)                             |
|AI        |Anthropic Claude API (claude-sonnet-4-20250514)            |
|Deployment|GitHub Pages                                               |
|Data      |Hardcoded Philly org/resource knowledge base + AI synthesis|

No database. No backend server. No tracking. Fully client-side except for the Anthropic API call.

-----

## Project Structure

```
climate-civic-advisor/
├── index.html          # Full deployable tool (React via CDN)
├── README.md           # You are here
├── METHODOLOGY.md      # AI prompt design, equity framing, org curation rationale
├── DATA_SOURCES.md     # Every Philadelphia organization and program referenced
├── CONTRIBUTING.md     # How orgs and residents can suggest additions
└── LICENSE             # MIT
```

-----

## Running Locally

This tool requires an Anthropic API key passed via the browser. To run locally:

1. Clone the repo:
   
   ```bash
   git clone https://github.com/meyeringn/climate-civic-advisor.git
   cd climate-civic-advisor
   ```
1. Open `index.html` in your browser. The tool uses the Anthropic API directly from the client — you’ll need a valid API key configured in the Claude.ai artifact environment, or modify the fetch call to include your key for local testing.
1. For GitHub Pages deployment, push to `main` and enable Pages from the repo settings (root directory).

-----

## Deploying to GitHub Pages

1. Go to your repo → **Settings** → **Pages**
1. Set source to **Deploy from a branch** → `main` → `/ (root)`
1. Save. Your tool will be live at `https://meyeringn.github.io/climate-civic-advisor` within a few minutes.

-----

## Part of the Vibe Coding for Climate Justice Series

This tool is part of a growing portfolio of civic tech projects built for Philadelphia and beyond:

|Project                                                                            |Description                                                   |
|-----------------------------------------------------------------------------------|--------------------------------------------------------------|
|[CanopyWatch](https://github.com/meyeringn/canopywatch)                            |36-neighborhood Philadelphia tree canopy equity dashboard     |
|[FloodRisk Philly](https://github.com/meyeringn/floodrisk-philly)                  |FEMA NFHL flood risk mapping tool                             |
|[SustAInable](https://github.com/meyeringn/sustainable-heat)                       |XGBoost model predicting neighborhood heat illness risk by ZIP|
|[UpLift](https://github.com/meyeringn/uplift-transit)                              |Predictive maintenance for SEPTA accessibility equipment      |
|[Transit Carbon Calculator](https://github.com/meyeringn/transit-carbon-calculator)|Statewide PA transit emissions calculator                     |
|[Climate Burden Index](https://github.com/meyeringn/climate-burden-index)          |Composite vulnerability index by Philadelphia ZIP code        |

-----

## Author

**Nico Meyering, MPA**

- Chairman, Philadelphia Mayor’s Commission on People with Disabilities
- VP of Growth & Partnerships, Net Impact Philadelphia
- Steering Committee, Transit Forward Philadelphia
- Board Member, Disability Pride Pennsylvania

[LinkedIn](https://linkedin.com/in/nicolasmeyering) · [GitHub](https://github.com/meyeringn)

-----

## License

MIT License — see <LICENSE> for details. Built for community use. Fork it, adapt it, deploy it for your city.