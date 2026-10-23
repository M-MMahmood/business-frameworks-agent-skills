# Business Frameworks: Agent Skills

A library of 26 agent skills for the strategy and consulting frameworks used most often in MBB-style engagements. Each skill gives an AI agent a repeatable process, an output format, and a quality checklist for one framework.

## Repository Structure

**Convention:** `<section>/<framework>/<framework>.md`

## Skill Index

| Section | Frameworks |
|---|---|
| 01 Strategy and Competitive Analysis | Porter's Five Forces, SWOT, PESTEL, 3Cs, VRIO, Generic Strategies, Scenario Planning |
| 02 Growth and Portfolio Decisions | Ansoff Matrix, BCG Matrix, GE-McKinsey Nine-Box, Three Horizons, Blue Ocean |
| 03 Business Model and Value Creation | Business Model Canvas, Lean Canvas, Value Chain, Profitability Framework |
| 04 Organization, Change and Performance | 7S, Balanced Scorecard, OKRs, Kotter's 8 Steps, Pyramid Principle, SMART/5W1H |
| 05 Marketing and Customer | 4Ps, STP, Customer Journey Mapping, NPS |

## Anatomy of a Skill

Every skill file uses the same layout:

1. **Frontmatter:** `name` and `description`, which an agent uses to decide when to load the skill.
2. **Purpose and When to use:** the triggers for the skill.
3. **Before you start:** the context and data to confirm first.
4. **Process:** numbered steps to follow.
5. **Output format:** the deliverable's structure.
6. **Common pitfalls:** typical mistakes to avoid.
7. **Quality checklist:** a final self-check.

## Usage

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/business-frameworks-agent-skills.git
   ```
2. Copy the skills you need into your agent's skills directory, or point your agent at this repo.
3. Prompt the agent naturally, for example: *"Run a Porter's Five Forces analysis on the US electric-vehicle charging industry."*

> **Compatibility note:** Some platforms (for example, Claude Skills) only load files named `SKILL.md`. If your platform requires that, rename each `<framework>.md` to `SKILL.md`. The frontmatter works unchanged.

## Contributing

1. Fork the repo and create a branch: `git checkout -b add-<framework-name>`.
2. Add a folder named in lowercase with hyphens, containing a file of the same name.
3. Follow the skill anatomy above.
4. Open a pull request with a short description and an example prompt.

**Naming rules:** lowercase, hyphen-separated, no spaces or special characters (`&`, `'`).

## License

Add a license of your choice, such as MIT, in a `LICENSE` file.

## Disclaimer

These skills describe publicly known frameworks. They are not affiliated with or endorsed by McKinsey & Company, BCG, Bain, or any framework author.
