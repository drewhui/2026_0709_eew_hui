# AI Agents and LLMs in Next-Generation Earthquake Early Warning

- Date: 2026-06-03  |  Venue: Taipei University of Municipal Affairs
- Speaker: Da-Yi Chen  |  Organization: CWA Seismological Center

---

## Taiwan Seismic Risk

- Philippine Sea Plate vs. Eurasia: **7-8 cm/yr** convergence
- ~**100 earthquakes/day**, ~**100 felt/yr**, major disaster every **30-40 yr**
- ~**3000 observation channels**, 100Hz sampling

### Recent Major Disasters
| Date | Event | Impact |
|------|-------|--------|
| 2016/02/06 | M6.6 Meinong | 1069 casualties |
| 2018/02/06 | M6.2 Hualien | 308 casualties |
| 2024/04/03 | M7.1 Hualien | 621 casualties |
| 2025/01/21 | M6.4 Dapu | 1810 houses damaged |

---

## EEW Architecture

### Pipeline
Detect P-wave -> Grouping -> Location -> Magnitude -> Intensity

### ML for Intensity
- Use **3 sec P-wave**, ~**15 sec leading time**

---

## Large Earthquake Model (LEM)

### SeisWav2Vec 2.0
- Adapted from Wav2Vec 2.0 (speech), contrastive learning
- Self-supervised: extracts features from unlabeled data

### Components
1. Feature Encoder: waveform -> embeddings
2. Context Encoder: 12-layer Transformer
3. Masking & Quantization: masked prediction

### Workflow
Pre-training (unlabeled) -> Fine-tuning (CNN Decoder) -> Inference

---

## Hermes Multi-Agent System

| Agent | Role | Responsibilities |
|-------|------|-----------------|
| my_agent | EEW Manager | Cron, anomaly alerts, daily summary |
| secondary_agent | Integration Engineer | Hermes forwarding, task dispatch |
| seismo_agent | Seismology Assistant | .rep parsing, latency, plots |
| seismo | Researcher | Modeling, experiments, trends |

### Automated Workflow
Event trigger (.rep) -> Data dispatch -> Plotting -> Modeling -> Report

---

## AI Workflow Evolution

| Period | Phase | Key Feature |
|--------|-------|-------------|
| 2022-2024 | Chat Era | ChatGPT, AI as assistant |
| 2024-2025 | IDE Integration | Cursor, Windsurf, Copilot Agent |
| 2025-2026 | Autonomous Agents | OpenClaw, Hermes, Claude Code |

---

## Conclusion
- SSL enables feature extraction from unlabeled data
- LEM brings new era for seismic monitoring
- Multi-agent collaboration reshaping EEW workflows
