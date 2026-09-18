# Nabla Linux

Product home for **Nabla OS** — full disk images for Raspberry Pi and Desktop.

| Deliverable | Description |
|-------------|-------------|
| **Nabla OS Pi** | Full disk image: Raspberry Pi OS with the Nabla layer pre-installed. |
| **Nabla OS Desktop** | Full disk image: Linux Mint with the same Nabla layer. |

Public docs and downloads live at [nabla.net/linux](https://nabla.net/linux). Apt packages are published under `/linux/apt` (mirror of the fleet apt). Base OS updates come from upstream distro repos (Raspberry Pi OS / Mint / Ubuntu); this repo documents the Nabla-specific layer that sits on top.

## Layout

```
images/      # image build scripts (Pi + Desktop)
profiles/    # core, inference (NVIDIA), kiosk, …
docs/        # site content for nabla.net/linux
apt/         # notes / CI for apt publishing (not the binary pool)
```

## Installing Nabla Edge on an existing system

If you have an existing Raspberry Pi OS or Linux box and want to join **Nabla Net** without reflashing, install the **Nabla Edge** package from the apt repository. Edge provides vpn-mode, Tailscale helpers, and firstboot hooks.

Edge package sources and development live in a separate repository:
**[txemavs/nabla-edge](https://github.com/txemavs/nabla-edge)**

## Related

| Resource | Link |
|----------|------|
| Nabla Edge (package sources + runtime) | [txemavs/nabla-edge](https://github.com/txemavs/nabla-edge) |
| Apt mirror / fleet packages | `nabla.net/linux/apt` |

Product UI and on-device strings: clear professional English. Operator chat may be Spanish.
