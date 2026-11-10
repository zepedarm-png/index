# Project AI Trainer — UI Preview

A responsive, interactive **frontend preview** for Project AI Trainer, published to Vercel from the `trainer-ui/` folder of this repository.

## What it includes

- Overview: project metrics for the eight-module curriculum and safe next-step links
- Module library: all eight coaching pillars and 56-case content architecture
- Conversation lab: a **fictional scripted demo** with typed agent replies
- Trainer review: five-criterion weighted scoring example, based on each module's rubric
- Reports: an **illustrative** graph and planned reporting fields
- Settings: transparent future integration status and browser-only display preferences

## Security and scope

This is a public **UI-only preview**, not the private AI scenario engine. No protected baseline or reassessment prompts, scenario hidden facts, actual learner records, API credentials, or server-side evaluation code are shipped.

**Do not add** `.env.local`, OpenAI keys, employee data, authentication tokens or private assessment JSON to this repository. Do not collect real customer data from the browser preview.

The full scenario engine v0.4 remains in the user's private working package and Google Drive; a secure backend must be built before connecting it to the public Vercel app.

## Local preview

No dependencies or build step:

```sh
python -m http.server 8080 --directory trainer-ui
```

Then visit `http://localhost:8080`.

## Deployment

Vercel project root directory: `trainer-ui`.

Framework preset: Other / static. The Vercel Git integration deploys this directory on updates to `main`.

## Planned integration

1. Authenticated learner and trainer access, with tenant separation.
2. Server-side scenario bank and state machine.
3. Model-backed customer simulator; private `OPENAI_API_KEY` configured server-side.
4. Evidence-linked evaluator and coaching engine after human calibration.
5. Voice input/output and supervised user acceptance testing.

All charts and rubric scores here are illustrative.