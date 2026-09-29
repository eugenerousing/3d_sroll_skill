# scroll-world (skill)

A copy of the **`scroll-world`** agent skill — builds an immersive scroll-scrubbed
"fly through the world" landing page: AI-generated scene stills, a seamless
camera-video chain (dive-ins + connectors), and a portable vanilla-JS scroll-scrub
engine with no visible cuts.

## Files

- `SKILL.md` — the full skill definition (the scroll-world instructions).

## ⚠️ Missing `references/` files

`SKILL.md` references five files under `references/` that are **not included** in
this repository, because they were not present in the source this copy was taken from:

| File | Purpose |
|---|---|
| `references/prompts.md` | intake checklist + prompt templates (scene still, dive, connector) |
| `references/pipeline.md` | copy-paste batch scripts (generate → extract frames → connectors → encode → mobile encode) |
| `references/scrub-engine.js` | the portable, config-driven scroll-scrub engine |
| `references/index-template.html` | minimal standalone page that mounts the engine |
| `references/knockout.py` | border-connected background knockout for floating scenes |

The skill **will not run end-to-end** until these are added. If you have the
originals, drop them into a `references/` folder and the skill is complete.

## Install / use as an agent skill

Conventional layout for an agent skill (folder named after the skill, containing
`SKILL.md`):

```
scroll-world/
  SKILL.md
  references/
    prompts.md
    pipeline.md
    scrub-engine.js
    index-template.html
    knockout.py
```

The `scroll-world` skill targets any framework — the scrub engine is self-contained
vanilla JS, so it drops into plain HTML, Next.js, Vue, or a Python-served page.
