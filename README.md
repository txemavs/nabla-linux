# Nabla Linux

Product home for **Nabla OS** and **Nabla Edge**.

| Piece | What it is |
|-------|------------|
| **Nabla OS** | Full disk image: Pi flavour (Raspberry Pi OS + Nabla layer) and Desktop flavour (Linux Mint + same layer). |
| **Nabla Edge** | Minimal `.deb` / package you install on an existing Pi OS or Linux box to join **Nabla Net** (vpn-mode, Tailscale helpers, firstboot hooks). |

Public docs and downloads will live at [nabla.net/linux](https://nabla.net/linux). Apt packages are published under `/linux/apt` (mirror of the fleet apt on Coco). Base OS updates still come from Raspberry Pi / Mint / Ubuntu repos; this repo only carries Nabla packages.

## Layout (planned)

```
packages/nabla-edge/   # minimal Edge package
images/                # image build scripts (Pi + Desktop)
profiles/              # core, inference (NVIDIA), kiosk, …
docs/                  # site content for nabla.net/linux
apt/                   # notes / CI for apt publish (not the binary pool)
```

## Related

- Fleet / Edge runtime: `txemavs/nabla-edge` (may fold package sources here over time)
- Packages share: `\\coco\nabla.net\`

Product UI and on-device strings: clear professional English. Chat with operators may be Spanish.
