# AI Feature Specs

Production-ready AI feature spec templates for PMs and founders — with evaluation, safety, and rollout built in.

**Maintained by [Sumit Soni](https://github.com/isumitsoni) · [LinkedIn](https://linkedin.com/in/isumitsoni)**

---

## Why this repo exists

Most AI product docs stop at "what to build." This repo adds what usually gets skipped: eval gates, safety controls, rollout criteria, and cost/latency budgeting — all in one spec format, ready to hand to an engineering team.

---

## Who this is for

- PMs owning AI feature outcomes end-to-end
- Non-technical founders shipping AI products without a full engineering team

---

## What's included

| Template | Use case |
|----------|----------|
| [rag-search-feature.md](./rag-search-feature.md) | RAG-powered search or Q&A |
| [summarization-feature.md](./summarization-feature.md) | Document or content summarization |
| [classification-routing.md](./classification-routing.md) | Input classification or intent routing |
| [content-generation.md](./content-generation.md) | AI-assisted drafting or autocomplete |
| [conversation-agent.md](./conversation-agent.md) | Conversational AI / chatbot |
| [recommendation-engine.md](./recommendation-engine.md) | Personalized recommendations |

Each template includes:
- Problem + target user
- Inputs and outputs (with fill-in examples)
- Happy path behavior + edge cases
- Model strategy (primary / fallback / escalation)
- Evaluation plan (rubric + golden dataset + stage thresholds)
- Safety and policy controls
- Rollout gates (alpha → beta → GA)
- Cost and latency budget section
- Open questions to resolve before engineering kickoff

---

## How to use

1. Duplicate the closest template for your feature type.
2. Fill every bracketed field before kickoff.
3. Resolve open questions before writing production code.
4. Set eval thresholds before implementation starts — not after.
5. Use rollout gates as explicit go/no-go criteria.

---

## Contributing

PRs welcome if they include:
- A real AI feature pattern not yet covered
- Concrete failure modes and detection methods
- Eval rubric with specific dimensions (not generic "quality")

No generic templates without eval logic.

---

## Related repos

- **[pm-prompts](https://github.com/isumitsoni/pm-prompts)** — Prompt library for every PM workflow, including AI feature specs
- **[awesome-ai-pm](https://github.com/isumitsoni/awesome-ai-pm)** — Curated AI PM resources and tools
- **[vibe-coding-playbook](https://github.com/isumitsoni/vibe-coding-playbook)** — Cross-tool build playbooks for PMs and founders

---

*Star this repo if it saves you time in a kickoff or review meeting.*
