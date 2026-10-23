<p align="center">
  <h1 align="center">Neuro_Morph</h1>
  <p align="center">
    <strong>Experimental neural networks whose internal states and senses regulate how their own connections change</strong>
  </p>
  <p align="center">
    <img src="https://img.shields.io/badge/status-research_phase-orange?style=flat-square" alt="Status">
    <img src="https://img.shields.io/badge/research-22_topics_verified-brightgreen?style=flat-square" alt="Research">
    <img src="https://img.shields.io/badge/focus-neuromodulated_plasticity-blue?style=flat-square" alt="Focus">
    <img src="https://img.shields.io/badge/GPU-RTX_5080_16_GB-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="GPU">
  </p>
</p>

---

Neuro_Morph investigates whether an artificial neural network can learn and adapt better when **emotion-like internal states and sensory experience change how its connections work and how they learn**, instead of being fed in as ordinary inputs. The same event should be able to produce a different response depending on the network's history, its current state and who is involved, the way a person who hates surprises can still be thrilled by a surprise from someone they love.

## Project Scope

**This project is:**
- A research project on state-dependent, experience-dependent plasticity in small neural networks
- Built around three adaptation layers: temporary modulation, experience-dependent learning, and (later) structural change
- Designed around an explicit emotion model: emotion vectors, situation-dependent intensity, and appraisal shaped by past experience and relationships
- Measured against matched baselines, with negative results counted as results
- Developed and run locally on a single consumer GPU

**This project is NOT:** a large general-purpose language model, a claim of machine consciousness or felt emotion, or a scripted "act emotional" chatbot.

## Core Idea

```
W_effective(t) = W_base + W_modulated(t) + W_plastic(t)
```

| Component | Role |
|---|---|
| `W_base` | Slow, stable knowledge (long-built "ideals") |
| `W_modulated(t)` | Temporary change driven by the current internal state; leaves no lasting trace |
| `W_plastic(t)` | Experience-dependent change gated by emotion-like signals; can persist and decay |

The question every experiment answers: does letting internal state regulate the connections beat a network that receives the same state only as an extra input?

## Research

Before any code, every idea behind the project was checked against the literature. 22 topics (13 of the owner's own claims, 9 factors the original design did not mention) were each researched by a separate agent and passed an adversarial critic that opened every source.

- [Research summary and design principles (Turkish)](docs/research/README.md)
- [Full topic reports](docs/research/konular/)

## Phases

| Phase | Description | Status |
|-------|-------------|--------|
| 0. Research | Scientific basis of every design claim, verified sources | ✅ Done |
| I. Foundations | Small networks with state-dependent modulation and elementary plasticity; numerical checks against the math | 🔲 Planned |
| II. Learning and adaptation | Environments where senses, internal state and feedback drive learning; comparison against baselines | 🔲 Planned |
| III. Memory and structure | Short vs long-term adaptation, consolidation, controlled connectivity change | 🔲 Planned |
| IV. Small language model | The most promising mechanisms inside a compact language model trained from scratch | 🔲 Planned |

## Repository Layout

```
docs/
  research/           research summary, verdict table, design principles
    konular/          one full report per topic (T01 to T13, K1 to K4, G1 to G5)
```

## Hardware Target

- GPU: NVIDIA RTX 5080 (16 GB VRAM)
- CPU: AMD Ryzen 9800X3D
- RAM: 64 GB DDR5
- OS: Windows 11

---

<p align="center">
  <sub>Small networks, honest baselines, every claim checked.</sub>
</p>
