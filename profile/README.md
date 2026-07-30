```text
 _   _ ______
| | | || ___ \
| |_| || |_/ /
|  _  ||    /
| | | || |\ \
\_| |_/\_| \_|
```

# Hizrian Raz

**Philosopher · Wanderer · Neurodivergent · Founder**

Builder of [Ainfera](https://www.ainfera.ai) — honest inference routing.  
I measure what actually runs on one box, then publish the receipts — not the hype.

<p align="left">
  <a href="https://www.ainfera.ai"><img alt="Ainfera" src="https://img.shields.io/badge/Ainfera-ainfera.ai-0B1020?style=for-the-badge&labelColor=111827" /></a>
  <a href="https://x.com/hizrianraz"><img alt="X" src="https://img.shields.io/badge/X-@hizrianraz-111827?style=for-the-badge&logo=x&logoColor=white" /></a>
  <a href="https://huggingface.co/hizrianraz"><img alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-hizrianraz-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" /></a>
  <a href="https://github.com/hizrianraz"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-hizrianraz-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---

## Now

I keep a **personal measured stack** for one [DGX Spark](https://www.nvidia.com/en-us/products/workstations/dgx-spark/) (GB10 · 128 GB).

Packs are scripts, pins, cards, and eval receipts.  
**Not finetunes. Not company IP. Not invented numbers.**

| | Pack | Role | Status |
| ---: | --- | --- | --- |
| 1 | **[Laguna-S-2.1](https://github.com/hizrianraz/Laguna-S-2.1-Spark-Agentic)** | Long-horizon **repo maintenance** · official Q4_K_M | Measured day-0 · [HF](https://huggingface.co/hizrianraz/Laguna-S-2.1-Spark-Agentic) |
| 2 | **[Qwen3-Coder-Next](https://github.com/hizrianraz/Qwen3-Coder-Next-Spark-Agentic)** | Interactive **throughput** · quality FP8 | Day-0 path · [HF](https://huggingface.co/hizrianraz/Qwen3-Coder-Next-Spark-Agentic) |
| 3 | **[DeepSeek-V4-Flash REAP25](https://github.com/hizrianraz/DeepSeek-V4-Flash-REAP25-Spark-Agentic)** | Long-context **investigation** · REAP25/Pulsar | Experimental · **no hero** · [HF](https://huggingface.co/hizrianraz/DeepSeek-V4-Flash-REAP25-Spark-Agentic) |

Also on Mac (not Spark heroes):  
[Laguna-XS-2.1](https://huggingface.co/hizrianraz/Laguna-XS-2.1-Mac-Agentic) · [Qwen3-Coder-30B-A3B](https://huggingface.co/hizrianraz/Qwen3-Coder-30B-A3B-Mac-Agentic)

<details>
<summary><strong>Size · pins · windows</strong> (expand)</summary>

<br/>

**Window (WIB)**  
List target `2026-08-03 12:00` · freeze target `2026-08-02 18:00`  
Both clocks stay blocked until local HOLD lifts.

**Hero CTAs (sequential)**  
Laguna `Aug 3 20:00` → Qwen `Aug 4 20:00` → DeepSeek `null` (NO_HERO default)

**Laguna day-0 measured artifact**  
`hizrianraz/Laguna-S-2.1-GGUF` · `laguna-s-2.1-Q4_K_M.gguf`  
sha256 `a8b55c75714ea73fd90ec85de5defdc0b8d88ca0ad2108343cdd8fc22f7583e4`  
engine pin `04b2b72` (`poolside/llama.cpp-laguna`) · measure tip `bf82eab`  
format/routing smoke 40/40 · hermes 27/27 · ~21.47 t/s gen128  
→ **not** long-horizon agent reliability proof · DFlash/NVFP4 **not** day-0 flagship

**Upstream / quality refs** (not day-0 serve authority)  
[poolside/Laguna-S-2.1-NVFP4](https://huggingface.co/poolside/Laguna-S-2.1-NVFP4) · [Qwen/Qwen3-Coder-Next-FP8](https://huggingface.co/Qwen/Qwen3-Coder-Next-FP8) · [twaggs88 REAP25 DSpark GGUF](https://huggingface.co/twaggs88/DeepSeek-V4-Flash-REAP25-DSpark-ds4-GGUF) · bases [Laguna-S-2.1](https://huggingface.co/poolside/Laguna-S-2.1) · [Qwen3-Coder-Next](https://huggingface.co/Qwen/Qwen3-Coder-Next) · [DeepSeek-V4-Flash](https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash)

</details>

---

## How I work

```text
measure  →  pin  →  publish receipts  →  refuse the stretch claim
```

- **Conviction over consensus** — one box, real digests, reproducible scripts  
- **Verify the premise** — smoke ≠ headline · verifier ≠ gate clearance  
- **Honest labels** — experimental stays experimental until dated measure lands  

Public claim binder for every Spark pack:  
[`SPARK_AGENTIC_QUANT_STANDARD.md`](./SPARK_AGENTIC_QUANT_STANDARD.md) (SAQS)

<details>
<summary><strong>Honesty locks</strong> (always on)</summary>

<br/>

- `diy_gguf = false` — Laguna GGUF mirror hosts **official Poolside** bytes only  
- `public_promo_before_launch = false`  
- smoke ≠ agent headline · evidence-bind ≠ gate  
- Qwen day-0 forte = **FP8 quality** (not NVFP4 speed)  
- DeepSeek day-0 = scaffold / experimental · **NO_HERO** default  
- DSpark ≠ DGX Spark · peer GGUF ≠ full official DeepSeek V4 Flash (~155 GiB no-fit on one Spark)  
- Packs are **not** Ainfera routing, company eval, sales SKUs, or open finetunes  

</details>

---

## Reproduce (shape)

1. Open a pack `README` + `INSTALL.yaml`  
2. Pull the **named upstream** (or Laguna official GGUF + pack `SHA256SUMS`)  
3. Run `scripts/serve_*.sh` on **one** DGX Spark  
4. Diff your receipts under `results/` — smoke ≠ headline  

---

## Elsewhere

| | |
| --- | --- |
| Company | [ainfera.ai](https://www.ainfera.ai) · [@ainfera-ai](https://github.com/ainfera-ai) |
| Models | [huggingface.co/hizrianraz](https://huggingface.co/hizrianraz) |
| Profile mirror | [huggingface.co/hizrianraz/profile](https://huggingface.co/hizrianraz/profile) |
| Contact on packs | open a discussion on the relevant HF repo |

---

<sub>
Personal · unaffiliated measurement surface · not Ainfera product IP  
Index polished 2026-07-30 · measure authority held at Laguna tip <code>bf82eab</code>
</sub>
