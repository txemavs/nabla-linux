# Nabla Linux

Product home for **Nabla OS** disk images and documentation at [nabla.net/linux](https://nabla.net/linux).

## Three Installation Paths

| Path | What you get | Base system |
|------|--------------|-------------|
| **Nabla OS** | Full disk image with Nabla layer pre-installed | Flash and boot |
| **Nabla Edge only** | Join Nabla Net on an existing Pi or Linux box | Any Raspberry Pi OS / Debian / Ubuntu |
| **Nabla Inference only** | GPU inference sharing on NVIDIA machines | Any Linux with NVIDIA drivers |

## Nabla OS Flavours

| Flavour | Base | Use case |
|---------|------|----------|
| Nabla OS Pi | Raspberry Pi OS | Raspberry Pi devices |
| Nabla OS Desktop | Linux Mint | x86-64 desktops/servers |

Both flavours include the Nabla layer (Edge + profiles) out of the box.

## Sibling Packages

These packages live in their own repositories and can be installed standalone—no Nabla OS required:

| Package | Repository | Purpose |
|---------|------------|---------|
| **nabla-edge** | [txemavs/nabla-edge](https://github.com/txemavs/nabla-edge) | Raspberry Pis and Linux terminals: Nabla Net/VPN, Voice Assistant, kiosk mode. Install on any existing Linux. |
| **nabla-inference** | [txemavs/nabla-inference](https://github.com/txemavs/nabla-inference) | NVIDIA GPU machine sharing inference with the network. Requires careful access permissions. |

## Layout

```
images/      # Image build scripts (Pi + Desktop flavours)
profiles/    # Install profiles: core, inference, kiosk
docs/        # Site content for nabla.net/linux
apt/         # Notes for apt publish (not the binary pool)
```

## Apt Repository

Machines keep their distro base repos (Raspberry Pi OS / Mint / Ubuntu) **and** the Nabla apt source:

- **Public mirror:** `https://nabla.net/linux/apt`
- **Authoritative pool:** Coco fleet apt (`\\coco\nabla.net\apt`)

Base OS updates come from upstream; Nabla packages come from the Nabla apt.

## Related

- Public site: [nabla.net/linux](https://nabla.net/linux)
- Nabla Edge package: [txemavs/nabla-edge](https://github.com/txemavs/nabla-edge)
- Nabla Inference package: [txemavs/nabla-inference](https://github.com/txemavs/nabla-inference)
