# CogOS Research

**Part of the [CogOS](https://github.com/myrgic) ecosystem -- why it WORKS.**

Theoretical foundations, architecture research, and proof-of-concept experiments for cognitive operating system design.

Prior art here is cited where we know it. If you know of work we should be citing,
open an issue.

## Contents

| Document | Description | Last verified |
|----------|-------------|---------------|
| [papers/second-order-observability/](papers/second-order-observability/) | **Second-Order Observability** -- declared observability is optional while the observer is more reliable than the referent, and mandatory once it is not. Frozen thesis, prior-art verdict, 12 primary-source-verified claims, and a runnable demonstrator. Paper in progress. | 2026-09-12 |
| [src/](src/) | **Self-Referential Closure (SRC)** -- the model equations, the survivors (τ₁ = ln(2), a = 6, θ-invariance), and cross-domain instantiations. Scoped deliberately; see the note in that README about the wider framework. | 2026-05-08 |
| [eaefm/thesis.md](eaefm/thesis.md) | **EA/EFM Thesis** -- Externalized Attention and Executive Function Modulation. The core argument: the substrate thinks, the model generates, and quality is a function of boundary quality. | 2026-05-08 |
| [loro/framework.md](loro/framework.md) | **LoRO Framework** -- Low-Rank Observer as a framing connecting PLE (Per-Layer Embeddings), LoRA (Low-Rank Adaptation), and TRM (Tiny Recursive Model). Three mechanisms, one pattern, operating at different time scales. | 2026-05-08 |
| [poc/](poc/) | Two proof-of-concept design notes: dormant inference cascade, semantic coherence. Designs, not results. | 2026-04-07 |

"Last verified" is when the claims were last checked, not when the file was last edited.

## What this is

This repo contains public research from Myrgic Labs. Most of it underpins CogOS -- the
ideas about *why* externalizing attention and executive function into a substrate
produces better outcomes than scaling model size alone. The `papers/` lane is broader:
work intended for outside readers, which may or may not be about CogOS.

The key claims:

1. **EA (Externalized Attention):** Deciding what information is relevant *before* the model sees it -- not retrieval, not augmentation, but selective amplification of what matters.
2. **EFM (Executive Function Modulation):** Deciding how the model should behave *before* it generates -- not prompting, but shaping the computational trajectory through conditioning signals.
3. **LoRO (Low-Rank Observer):** PLE, LoRA, and TRM as instances of one pattern -- low-rank conditioning of a larger system through a bottleneck, operating at different time scales.

## What this is not

This is public architecture research related to CogOS. It does not contain the full theoretical framework, fundamental physics, or private workspace internals.

## Related projects

- [cogos](https://github.com/myrgic/cogos) -- The kernel — continuous process daemon with foveated context and multi-provider routing
- [constellation](https://github.com/myrgic/constellation) -- Distributed trust — identity as temporal coherence, O(1) mutual verification
- [mod3](https://github.com/myrgic/mod3) -- Modality bus — translates between thinking and acting, voice-first
- [plugins](https://github.com/myrgic/plugins) -- Plugin marketplace — Agent Skills across workflow, research, voice, and dev tools
- [charts](https://github.com/myrgic/charts) -- Deployment — Helm charts + Docker Compose
- [desktop](https://github.com/myrgic/desktop) -- [ARCHIVED] Native macOS app -- kernel management, terminal, dashboard
- [openclaw-plugin](https://github.com/myrgic/openclaw-plugin) -- [ARCHIVED] OpenClaw integration (how it CONNECTS)

## License

MIT
