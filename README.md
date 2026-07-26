# Immersive Fusion Kids Academy

Source for **kids.immersivefusion.academy** — the kids' tier of the Immersive Fusion academy.

A small publication about AI, written for kids, by an observability company.

## What this is

The kids' tier of the academy. Where *Mosey and Wobble* and future kid-readable booklets live.

The academy exists to give anyone — kid or adult — a way to think about AI that is neither fear-mongering nor salvation-mongering. The frame is AI as ally: useful, fallible, requiring your own judgment. We don't sell on these pages.

A general-tier sibling site exists at [immersivefusion.academy](https://immersivefusion.academy), built from [if-academy-general-http](https://github.com/ImmersiveFusion/if-academy-general-http).

## License

This repository is licensed **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**. See [LICENSE](LICENSE).

Two notes on what the license is and isn't:

- **Booklets, essays, and the editorial charter are CC BY-NC 4.0.** Anyone can copy, print, translate, or build on this work for non-commercial purposes, with attribution. Schools, parents, and teachers can use any of it freely without asking. We do not want commercial reuse without permission.
- **Underlying reference materials** the publication cites (the AI tenets we follow, our link policy, the patterns we extract from our own writing) live elsewhere under **CC BY 4.0** so anyone can cite or build on them, including in commercial work that wants to align with the same posture.

The site's MkDocs configuration, theme overrides, and CI workflows are also covered by the repository license. MkDocs ([BSD-2-Clause](https://github.com/mkdocs/mkdocs/blob/master/LICENSE)) and [Material for MkDocs](https://github.com/squidfunk/mkdocs-material) (MIT) are attributed dependencies under their own upstream licenses.

## What this publication refuses to do

See [docs/about.md](docs/about.md). The editorial charter is the load-bearing document of the publication: dated, signed, and structurally identical to the general tier's charter. A reader who arrives skeptical can verify the publication's behavior against it.

## Local development

```pwsh
& .\envprep.ps1     # install dependencies
& .\serve.ps1       # serve locally on http://127.0.0.1:8000
```

Requires Python 3.12+.

## Deployment

Pushed to `main` deploys to **kids.immersivefusion.academy**. Hosted by Immersive Fusion at our cost. See [.github/workflows/deploy.yml](.github/workflows/deploy.yml).

## Repository conventions

This repository follows the `if-{property}-{type}-http` convention of [if-apm-documentation-http](https://github.com/ImmersiveFusion/if-apm-documentation-http) (the IF product documentation site). Sister repository: [if-academy-general-http](https://github.com/ImmersiveFusion/if-academy-general-http) for the adult tier at the academy root domain.

---

*by Immersive Fusion*