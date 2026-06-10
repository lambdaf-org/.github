<p align="center">
  <img src="https://raw.githubusercontent.com/lambdaf-org/.github/main/profile/lambdaforge-logo.png" alt="LAMBDAFORGE" width="500">
</p>

<h3 align="center">Tools that show their work.</h3>

<p align="center">
  <i>Software built to be used.</i><br>
  A workshop · open source · <a href="https://lambdaf.org">lambdaf.org</a>
</p>

---

## The tools

Each one is its own repository under `lambdaf-org`. Open the source and read how it works.

| # | Tool | Stack | What it does |
|--:|------|-------|--------------|
| 01 | [**Overseer**](https://github.com/lambdaf-org/overseer) | `Claude Code` · plain files | A second brain you reason with. Drop in your goals, the people around you, and your work, then ask what to focus on and get an answer drawn from one graph. It never stores status, and every claim carries a receipt. |
| 02 | [**Saul Swissman**](https://github.com/lambdaf-org/saul-swissman) | `Claude Code` · Swiss law | Answers on Swiss federal law where every statement carries the article, the SR number, the verbatim wording, and the consolidation date. No citation, no claim. When the corpus runs out, it points to Fedlex. |
| 03 | [**auspex**](https://github.com/lambdaf-org/auspex-v1) | `Rust` · local-only | Point it at your chat exports for cited per-person profiles and a real interaction graph. Every confidence number is computed from how many falsification probes a claim survived. Nothing leaves your machine. |
| 04 | [**synthesis**](https://github.com/lambdaf-org/synthesis) | `Python` · docs & audio | A folder of documents becomes a self-contained interactive HTML briefing, or live-transcribe a lecture into a structured report. An item ships only when two passes agree and it carries a grounded quote. |
| 05 | [**The Factory**](https://github.com/lambdaf-org/the-factory) | `Claude Code` · agent scaffold | Drop source into `context/`, write `task.md`, and run Claude Code as an autonomous worker. It keeps its own notes and resumes warm; output lands in a new `deliverable/` folder and your input is left untouched. |
| 06 | [**Neuro**](https://github.com/lambdaf-org/neuro) | `Rust` + `Vue 3` · real-time | Five short gamified cognitive tests over a real-time WebSocket pipeline, giving a five-part score profile with per-game leaderboards. Each game targets one narrow ability. |
| 07 | [**ClockBot**](https://github.com/lambdaf-org/clock) | `Rust` · Discord | Clock in and out of work activities from Discord slash commands and get weekly hours, rankings, and PNG charts back. Weekly stats archive every Monday. |
| 08 | [**transl**](https://github.com/lambdaf-org/transl_cli) | `Rust` · CLI | Add one key and value to your base-language JSON file and transl carries that key across every sibling language file, so your translations stay in sync. |
| 09 | [**MoneyForge**](https://github.com/lambdaf-org/MoneyForge) | `Next.js 16` · local-only | Track savings goals by name, target, balance, and monthly contribution, and see how many months each one needs. Browser-only, no backend, no accounts. |
| 10 | [**GradeForge**](https://github.com/lambdaf-org/GradeForge) | `Next.js 16` · local-only | Calculate your School Grade averages, any grading system, any country. Browser-only, no backend, no accounts. |

## The bench rules

How they are built. Not every tool does every one; where a tool makes a claim or touches your data, these hold.

1. **Receipts.** A claim about a person, a relationship, or the law carries a quote and a pointer back to the source, or it does not get written down. · `overseer` `saul-swissman` `auspex`
2. **Computed confidence.** Confidence is computed from counted evidence and shown with its tally. · `auspex` `overseer`
3. **Explicit about what leaves.** Your files stay on disk; the tools that reach a model strip secrets first and say what goes out. · `auspex` `synthesis` `overseer`
4. **No ceremony.** Several tools are one Markdown protocol with the model as the engine. Nothing to deploy, no schema, no service to babysit. · `overseer` `saul-swissman`

## The people

Everyone who has pushed commits to the tools above, drawn from each repository's history.

- [**@191-iota**](https://github.com/191-iota) · _Producing software people actually need._ · overseer, saul-swissman, auspex, synthesis, the-factory, neuro, clock, transl
- [**@Ajith1412**](https://github.com/Ajith1412) · neuro, clock
- [**@Thirstums**](https://github.com/Thirstums) · clock, GradeForge, MoneyForge

## Get started

Each tool is its own repository. Clone it, read the protocol or the source, and run it.

```bash
git clone https://github.com/lambdaf-org/<tool>
```

New here? Start with the [contributor guide](https://github.com/lambdaf-org/contributing).

<p align="center"><sub><a href="https://lambdaf.org">lambdaf.org</a> · open source under <a href="https://github.com/lambdaf-org">lambdaf-org</a> · 2026</sub></p>
