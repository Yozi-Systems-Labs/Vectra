# Vectra Public Documentation Site (`vectra-public`)

## 1. What is this repository?
**Component Name:** Vectra Public Documentation Portal (`vectra-public`)  
**Owner:** Yozi Systems Enterprise & Product Engineering  
**Scope:** Static documentation site and public distribution portal for Vectra™ / Advanced Tensor Governance System (ATGS), hosted at `yozi.systems/vectra`.

## 2. What problem does it solve?
Publishes public product documentation, diagnostic reviews, SDK reference manuals, and technical roadmaps for the Vectra CTMC tensor governance engine.

## 3. How is it built and tested?
- **Prerequisites:** Python 3.10+, MkDocs / `atgs-enterprise-core` build toolchain
- **Build & Test Commands:**
  ```bash
  # Site content is compiled from upstream atgs-enterprise-core documentation build
  cd /home/yozi/atgs-enterprise-core && cmake --build build --target site
  ```

## 4. Where is the canonical institutional documentation?
Canonical platform specifications, CTMC solver architecture reviews, and commercial positioning reside in central `yozi-docs`:
- 📍 **ATGS Platform Architecture:** [`yozi-docs/platform/atgs/`](file:///home/yozi/yozi-docs/platform/atgs/)
- 📍 **Commercial Positioning & Strategy:** [`yozi-docs/company/atgs_canonical_positioning_v1.md`](file:///home/yozi/yozi-docs/company/atgs_canonical_positioning_v1.md)
- 📍 **Open Core Strategy:** [`yozi-docs/company/atgs_open_core_strategy_v1.md`](file:///home/yozi/yozi-docs/company/atgs_open_core_strategy_v1.md)

## 5. Which repositories does it depend on?
- **Upstream Dependencies:** [`atgs-enterprise-core`](file:///home/yozi/atgs-enterprise-core) (source of MkDocs documentation and site generator)
- **Downstream Consumers:** Enterprise customers, CTMC solver evaluators, SDK integrators

## 6. Where should new documentation for this repository be placed?
- **Repository-Local Technical Documentation (`docs/` or `README.md`):** Shipped static web assets and GitHub Pages deployment configuration.
- **Central Institutional Documentation (`yozi-docs/`):** Strategic positioning, platform benchmarks, and CTMC solver architecture reviews (`yozi-docs/platform/atgs/`).
