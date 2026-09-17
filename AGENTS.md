# Agents

| Area | Owner |
|------|--------|
| Home Assistant / house | Dom |
| Pi images, vpn-mode, Nabla Net packages | Edge |
| ESP UI boards | Spui |
| Orchestration | Verónica |

This repo is the **Nabla Linux** product tree: Nabla OS images and docs for [nabla.net/linux](https://nabla.net/linux).

## Scope

This repo contains **only** image build configs, profiles, and documentation. Package sources live in sibling repos:

| Package | Repository | Standalone? |
|---------|------------|-------------|
| nabla-edge | [txemavs/nabla-edge](https://github.com/txemavs/nabla-edge) | Yes — installs on any Pi OS / Debian / Ubuntu |
| nabla-inference | [txemavs/nabla-inference](https://github.com/txemavs/nabla-inference) | Yes — any Linux with NVIDIA GPU |

Do not vendor package sources here. Keep `images/`, `profiles/`, `docs/`, `apt/` only.

## Style

Product / on-device strings: clear professional English. Operator chat may be Spanish.
