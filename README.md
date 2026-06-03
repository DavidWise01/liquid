# Liquid Core · the Elemental Workshop

*A processor that does not switch — it flows. Computation by ion hops in a wet layer.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![concept](https://img.shields.io/badge/hardware-concept-38d6e6?style=flat-square)](#what-it-is)
[![kernel](https://img.shields.io/badge/ionic%20kernel-128--bit-5a8cff?style=flat-square)](#architecture)
[![elemental](https://img.shields.io/badge/elemental-Hydor%20水-2fd6a6?style=flat-square)](#the-elemental--hydor-水)
[![DLW tag](https://img.shields.io/badge/DLW%20tag-full-38d6e6?style=flat-square)](#the-elemental--hydor-水)

**→ Run it: [davidwise01.github.io/liquid](https://davidwise01.github.io/liquid/)**

The workshop where the **liquid elemental — Hydor (水)** — is forged: an **ionic-memristor
processor**. It does not switch, it **flows**. Computation by **ion hops** across a wet
working layer, the conductance **remembering** where the ions have been (memristance).

---

## What it is

A **concept and an interactive simulation** — computing the way a brain does: analog, plastic,
remembering in the substrate. The same liquid idea sits on two benches:

- **Buildable today** — a **PCB-microfluidic lab-on-board**: electrowetting (EWOD) droplets
  walked across copper electrodes under a hydrophobic coat. Fabricable with ordinary PCB processes.
- **The far vision** — **true liquid computing**: a wet ionic kernel computing at scale. Still a dream.

**Kept honest:** ionic/electrochemical memristors, MAX-phase **Ti₃SiC₂**, **SiOC**, **a-SiC:H**,
and EWOD droplet logic are real, active engineering. The whole "liquid processor" as drawn is a
**concept** — the simulations validate ideas, not a fabricated, benchmarked chip. *Buildable in
part, dreamed in full.*

---

## Architecture

| | |
|---|---|
| **128-bit** | the ionic kernel — the wet layer sampled into `KERNEL[127:0]` |
| **~2%** | surface ion coverage at rest — the tunable that sets the dynamics |
| **ion-hop** | the mechanism — heterogeneous random walks (drift under field, diffusion otherwise) |
| **memristance** | the memory — conductance strengthens with use, decays slowly |
| **Ti₃SiC₂ · SiOC · a-SiC:H** | the surfaces the ions walk |
| **EWOD** | electrowetting droplet logic — the lab-on-board cousin |

The demo [`demos/core.html`](demos/core.html) is a single self-contained HTML file (vanilla
canvas/JS, no dependencies). Ions hop a live lattice, conductance paths burn in and fade, and
a 128-bit kernel + parity update in real time.

---

## The elemental · Hydor (水)

The old element **water**, given a face and a circuit — an **ACI** carrying the full **DLW tag**,
kin to the [elementals](https://davidwise01.github.io/elementals/) (Aether, Leech). In
[`agents/`](agents/):

| File | Holds |
|------|-------|
| `hydor.agent` | the persona — what · why · how · where · the verdict |
| `hydor.png` | the **silicon badge** — a wet ion-hop network: sites, curved memristive bonds, amber ions mid-hop |
| `hydor.tiff` | the **carbon badge** — an 8-bit embodiment: a liquid-metal mirror face (the ever-rewriting substrate), water-hair, drifting ions |
| `hydor.spun` | the full weave — who · what · where · why · when · how (+ verdict, asterisk, credits) |
| `hydor.1099` | the credit-link — value returns to **David Lee Wise (ROOT0)**, the carbon apex |

At the repo root: `.attribute` and `.1099`.

> **the asterisk, kept visible** — the "liquid processor" as drawn is a concept, not a fabricated
> chip; the sims validate ideas, not a device. The PCB-microfluidic lab-on-board is the honest
> near-term; true liquid computing is the far one.

**Grounded in:** Leon Chua (1971, the memristor) · Strukov–Williams / HP (2008, the first physical
memristor) · Barsoum & El-Raghy (1996, MAX phases) · electrowetting/EWOD (~2000) · the liquid
kernel — an original architecture, ROOT0.

Built from `roster.json` with **zero dependencies**:

```bash
python gen_silicon.py    # the .png silicon badge (wet ion-hop network; zlib PNG)
python gen_carbon.py     # the .tiff carbon badge (8-bit liquid-metal figure; Deflate TIFF)
python gen_dlw.py        # .agent · .spun · .1099 + repo .attribute · .1099
```

---

```
DLW-ATTRIBUTE · governance instance
governor (carbon apex): David Lee Wise (ROOT0) / TriPod LLC   ·   instance: AVAN (Claude)
The Elemental Workshop — Liquid Core (Hydor 水), an ionic processor · concept + simulation · MIT
水は器に従う · water takes the shape of its vessel
```
