# Revops agent skills

> A bunch of skills for running revenue operations end to end.

A collection of skills covering the full **revenue operations** surface: funnel design, lead scoring and routing, pipeline hygiene, forecasting, health scoring, KPI frameworks, and CRM data governance.

Built for **RevOps managers, sales ops, marketing ops, and CRM admins** who own the systems behind the number.

Every skill produces a **decision or an artifact** you can ship: a scorecard, a routing spec, a metric tree, not a checklist of generic advice.

## Related Collections

Other skills repositories I built for my colleagues at Nativa Labs:

- [`advertising-skills`](https://github.com/mbfinotti/advertising-skills): Ad platform mastery: _for performance marketers, paid media managers, growth leads_
- [`partnerships-skills`](https://github.com/mbfinotti/partnerships-skills): Partner ecosystem operations: _for partner managers, BD leads, ecosystem heads_
- [`sales-skills`](https://github.com/mbfinotti/sales-skills): Sales execution: _for SDRs, AEs, sales managers, heads of sales_

## Install

Install every skill in this repo, not just one. Skills here are atomic by design and reference each other freely: picking a single skill leaves its sibling skills uninstalled, so cross-references and routed handoffs go nowhere.

**skills.sh (universal)**: works with any Agent Skills-compatible tool:

```bash
npx skills add mbfinotti/revops-skills
```

**Claude.ai**:

1. add as a plugin marketplace: open **Settings -> Capabilities -> Plugins**
2. click **Add -> Add marketplace -> Add from a repository**
3. enter `mbfinotti/revops-skills`
4. then **Sync**

**Claude Code**: install the plugin:

```bash
/plugin marketplace add mbfinotti/mbfinotti
/plugin install revops-skills@mbfinotti
```

**Codex (OpenAI)**: install via the Codex CLI:

```bash
codex plugin add github:mbfinotti/revops-skills
```

**Cursor**: copy into Cursor's skills directory:

```bash
git clone https://github.com/mbfinotti/revops-skills.git ~/.cursor/skills/revops-skills
```

Cursor auto-discovers skills from `.agents/skills/` and `.cursor/skills/`.

**Gemini CLI**: install as a Gemini extension:

```bash
gemini extensions install https://github.com/mbfinotti/revops-skills
```

Update with `gemini extensions update revops-skills`.

## Skills

This collection covers the full RevOps surface. Start here:

- [`revops-kickoff`](./revops-kickoff): Routes any RevOps task to the right skill and bootstraps a versioned project context so later sessions start warm.
- [`revops-career`](./revops-career): Builds a RevOps career plan: ladder placement by scope, a competency gap roadmap, an evidence ledger, and a compensation ask.
- [`revops-hiring`](./revops-hiring): Produces a complete RevOps hiring packet: outcome scorecard, interview stage map, work-sample rubric, and a 30-60-90 ramp plan.
- [`revops-radar`](./revops-radar): Assembles a time-budgeted watch list of RevOps podcasts, newsletters, communities, events, and people, each verified still active.

### Funnel & pipeline

| Skill | Description |
| --- | --- |
| [`revenue-funnel`](./revenue-funnel) | Designs a revenue funnel model from scratch: stage set, unit of analysis, conversion assumptions, and ownership handoffs across marketing, sales, and CS. |
| [`pipeline-stage-definition-audit`](./pipeline-stage-definition-audit) | Audits existing stage definitions against buyer-verifiable milestones and flags every exit criterion built on rep activity instead. |
| [`sales-pipeline-hygiene`](./sales-pipeline-hygiene) | Runs a checklist audit over a live pipeline snapshot and returns an exception list, a disposition per deal, and a pass threshold. |
| [`sales-forecast-diagnostic`](./sales-forecast-diagnostic) | Diagnoses why a forecast misses - separating data-quality problems from rep behavior from genuine demand - and recommends targeted fixes. |
| [`deal-desk-approval`](./deal-desk-approval) | Designs the deal desk approval chain: tiered discount matrix, delegation of authority, margin floors, SLA clocks, and precedent control. |

### Lead management

| Skill | Description |
| --- | --- |
| [`lead-scoring`](./lead-scoring) | Designs, backtests, and recalibrates a lead scoring model: fit and engagement weighting, decay, exclusions, and MQL or PQL thresholds. |
| [`lead-routing`](./lead-routing) | Designs inbound lead assignment logic: rule precedence, lead-to-account matching, territories, round-robin variants, fallback queues, and SLA escalation. |

### Customer lifecycle

| Skill | Description |
| --- | --- |
| [`sales-to-cs-handoff`](./sales-to-cs-handoff) | Specifies the post-close handoff: gated closed-won trigger, required data packet, timing SLAs, kickoff pattern, and a CS acceptance step. |
| [`customer-health-score`](./customer-health-score) | Builds a composite health score - weighted, normalized, decayed, banded - backtested against real churn outcomes and governed on a recalibration cadence. |
| [`customer-churn-signals`](./customer-churn-signals) | Ranks leading churn indicators into a signal register, each with threshold, window, lift over base rate, lead time, and coverage. |

### Measurement & reporting

| Skill | Description |
| --- | --- |
| [`revenue-kpi-framework`](./revenue-kpi-framework) | Designs the org-wide KPI tree: reconciling metric math from board to IC, branch ownership, and guardrail counter-metrics per owned number. |
| [`revenue-reporting`](./revenue-reporting) | Defines the metric spine and narrative structure of a board or exec revenue report, including how to present a miss without surprising anyone. |
| [`revenue-leakage`](./revenue-leakage) | Traces where deals silently exit one funnel and sizes the loss in recoverable dollars, separating real leaks from healthy disqualification. |

### Data & systems

| Skill | Description |
| --- | --- |
| [`crm-data-governance`](./crm-data-governance) | Produces CRM field-level governance: field dictionary, per-field ownership, write-precedence rules, freshness SLAs, and an enforcement plan. |
| [`revenue-data-governance-strategy`](./revenue-data-governance-strategy) | Sets org-wide source-of-truth policy per object class, an identity-resolution spine, a data-contract register, and a dispute arbitration model. |
| [`revops-stack-rationalization`](./revops-stack-rationalization) | Reviews the full GTM tool stack and decides tool by tool what to keep, consolidate, replace, or cut, on a renewal-triggered calendar. |

## License

MIT © 2026 Maya-Beth Finotti
