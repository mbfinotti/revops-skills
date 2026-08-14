# Revops agent skills

> A bunch of skills for running revenue operations end to end.

A collection of skills covering the full **revenue operations** surface — funnel design, lead scoring and routing, pipeline hygiene, forecasting, health scoring, KPI frameworks, and CRM data governance.

Built for **RevOps managers, sales ops, marketing ops, and CRM admins** who own the systems behind the number.

Every skill produces a **decision or an artifact** you can ship: a scorecard, a routing spec, a metric tree, not a checklist of generic advice.

## Install

Install every skill in this repo, not just one. Skills here are atomic by design and reference each other freely — picking a single skill leaves its sibling skills uninstalled, so cross-references and routed handoffs go nowhere.

**skills.sh (universal)** — works with any Agent Skills-compatible tool:

```bash
npx skills add mbfinotti/revops-skills
```

**Claude Code** — install the plugin:

```bash
/plugin marketplace add mbfinotti/mbfinotti
/plugin install revops-skills@mbfinotti
```

**Codex (OpenAI)** — install via the Codex CLI:

```bash
codex plugin add github:mbfinotti/revops-skills
```

**Cursor** — copy into Cursor's skills directory:

```bash
git clone https://github.com/mbfinotti/revops-skills.git ~/.cursor/skills/revops-skills
```

Cursor auto-discovers skills from `.agents/skills/` and `.cursor/skills/`.

**Gemini CLI** — install as a Gemini extension:

```bash
gemini extensions install https://github.com/mbfinotti/revops-skills
```

Update with `gemini extensions update revops-skills`.

## Skills

This collection covers the full RevOps surface. Start here:

- [`revops-kickoff`](./revops-kickoff) — Routes any RevOps task to the right skill and bootstraps a versioned project context so later sessions start warm.
- [`revops-career`](./revops-career) — Builds a RevOps career plan — ladder placement by scope, a competency gap roadmap, an evidence ledger, and a compensation ask.
- [`revops-hiring`](./revops-hiring) — Produces a complete RevOps hiring packet — outcome scorecard, interview stage map, work-sample rubric, and a 30-60-90 ramp plan.
- [`revops-radar`](./revops-radar) — Assembles a time-budgeted watch list of RevOps podcasts, newsletters, communities, events, and people, each verified still active.

Browse all skills and their descriptions in [`references/skill-catalog.md`](./references/skill-catalog.md).

## Related Collections

Other Nativa Labs skill repositories:

- [`advertising-skills`](https://github.com/mbfinotti/advertising-skills) — Ad platform mastery — _for performance marketers, paid media managers, growth leads_
- [`partnerships-skills`](https://github.com/mbfinotti/partnerships-skills) — Partner ecosystem operations — _for partner managers, BD leads, ecosystem heads_
- [`sales-skills`](https://github.com/mbfinotti/sales-skills) — Sales execution — _for SDRs, AEs, sales managers, heads of sales_

## License

MIT © 2026 Maya-Beth Finotti
