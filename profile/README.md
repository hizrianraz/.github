# hizrianraz — personal measured stack (DGX Spark)

When people ask *"what measured stack do you actually run on one DGX Spark?"* — this is the honest index.

**Not Ainfera. Not a product line. Not company IP.**
Personal, unaffiliated measurement packs I maintain so I (and anyone reproducing) can pin digests, serve scripts, and receipts without inventing numbers.

## What this is

| Layer | Meaning |
| --- | --- |
| **Personal** | My own measured deployment notes on one DGX Spark (GB10, 128 GB). |
| **Unaffiliated** | No employer claim. No partnership claim. Upstream licenses still bind you. |
| **Pack** | Scripts + cards + eval receipts. **Not** a finetune. **Not** a re-quant publish by default. |

Day-0 surface = **these three packs**. Weight trees stay on their **official / peer upstream** IDs.

## Standard

Public claim binder: each pack ships `SPARK_AGENTIC_QUANT_STANDARD.md` (SAQS). Smoke ≠ headline under that standard.

## Honesty locks (always on)

- `diy_gguf = false` (Laguna GGUF mirror hosts **official Poolside** bytes only — pack ships digests + pull, not a DIY quant story)
- `public_promo_before_launch = false`
- smoke ≠ agent headline · verifier ≠ gate clearance · evidence-bind ≠ gate
- Qwen day-0 forte = **FP8 quality** (not NVFP4 speed) · DeepSeek day-0 = **scaffold / experimental**, **NO_HERO default**
- DSpark ≠ DGX Spark · peer GGUF ≠ full official DeepSeek V4 Flash (~155 GiB no-fit on one Spark)

## Family (Aug 3 window)

**List target:** 2026-08-03 12:00 WIB · **Freeze target:** 2026-08-02 18:00 WIB  
**Both clocks blocked** until local HOLD lifts (story surfaces match live Q4 authority; lock ban-phrases gone).

**Hero CTAs (sequential):** Laguna **Aug 3 20:00** → Qwen **Aug 4 20:00** → DeepSeek **hero null** (NO_HERO default; slot only if freeze **explicitly** re-opens HERO + dated measure).

| # | Pack | Role (honest) | Day-0 class | Hero CTA | Surfaces |
| --- | --- | --- | --- | --- | --- |
| 1 | **Laguna-S-2.1** | Long-horizon **repo-maintenance** · official **Q4_K_M** | **Measured** path on Q4_K_M + llama.cpp **04b2b72** · tip **bf82eab** (measure; docs tip advances separately) · format/routing smoke 40/40 · hermes 27/27 · ~21.47 t/s gen128 · **not** long-horizon agent reliability proof · DFlash/NVFP4 **not** day-0 flagship | Aug 3 20:00 WIB | [HF](https://huggingface.co/hizrianraz/Laguna-S-2.1-Spark-Agentic) · [GH](https://github.com/hizrianraz/Laguna-S-2.1-Spark-Agentic) |
| 2 | **Qwen3-Coder-Next** | Interactive **throughput + concurrency** · quality **FP8** | FP8 profile / preview probe · NVFP4 agent-cal = **post-launch** track only | Aug 4 20:00 WIB | [HF](https://huggingface.co/hizrianraz/Qwen3-Coder-Next-Spark-Agentic) · [GH](https://github.com/hizrianraz/Qwen3-Coder-Next-Spark-Agentic) |
| 3 | **DeepSeek-V4-Flash-REAP25** | Experimental **long-context investigation** · REAP25/Pulsar (~85 GiB) | Full official ~155 GiB **no-fit** one Spark · unmeasured scaffold · **NO_HERO** | **null** (no default hero) | [HF](https://huggingface.co/hizrianraz/DeepSeek-V4-Flash-REAP25-Spark-Agentic) · [GH](https://github.com/hizrianraz/DeepSeek-V4-Flash-REAP25-Spark-Agentic) |

**Authoritative measured artifact (Laguna day-0):**  
`hizrianraz/Laguna-S-2.1-GGUF` · `laguna-s-2.1-Q4_K_M.gguf`  
sha256 `a8b55c75714ea73fd90ec85de5defdc0b8d88ca0ad2108343cdd8fc22f7583e4` · engine pin `04b2b72` (poolside/llama.cpp-laguna)

**Upstream / quality references (not day-0 serve authority):**  
[poolside/Laguna-S-2.1-NVFP4](https://huggingface.co/poolside/Laguna-S-2.1-NVFP4) (post-launch track · DFlash **DO_NOT_PROMOTE**) · [Qwen/Qwen3-Coder-Next-FP8](https://huggingface.co/Qwen/Qwen3-Coder-Next-FP8) · [twaggs88 REAP25 DSpark GGUF](https://huggingface.co/twaggs88/DeepSeek-V4-Flash-REAP25-DSpark-ds4-GGUF) · bases [poolside/Laguna-S-2.1](https://huggingface.co/poolside/Laguna-S-2.1) · [Qwen/Qwen3-Coder-Next](https://huggingface.co/Qwen/Qwen3-Coder-Next) · [deepseek-ai/DeepSeek-V4-Flash](https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash)

**Also personal (Mac, not Spark day-0 heroes):**  
[Laguna-XS-2.1-Mac-Agentic](https://huggingface.co/hizrianraz/Laguna-XS-2.1-Mac-Agentic) · [Qwen3-Coder-30B-A3B-Mac-Agentic](https://huggingface.co/hizrianraz/Qwen3-Coder-30B-A3B-Mac-Agentic)

## What these packs are *not*

- Not open finetunes of the upstream checkpoints  
- Not a claim that “DIY GGUF = same quality”  
- Not a promise that peer REAP25/Pulsar equals full official DeepSeek V4 Flash  
- Not Ainfera inference routing, company eval, or a sales SKU  
- Not long-horizon agent reliability proof from format/routing smoke alone  
- Qwen FP8 ≠ NVFP4 speed claim · DeepSeek co-list ≠ full official on one Spark · DSpark ≠ DGX Spark

## Reproduce (shape)

1. Read the pack `README` + `INSTALL.yaml`  
2. Pull the **named upstream** (or the Laguna official GGUF mirror with pack `SHA256SUMS`)  
3. Run pack `scripts/serve_*.sh` on **one** DGX Spark  
4. Compare your receipts under `results/` — smoke ≠ headline  

## License / contact

Each pack carries upstream license text and `NOTICE`.  
Questions on **these personal packs only:** open a discussion on the relevant HF repo.

---
*Index rebuilt 2026-07-30T21:10:42+07:00 (A3 origin tips + measure tip split) · GitHub mirror: [hizrianraz/profile](https://github.com/hizrianraz/profile) · HF: [hizrianraz/profile](https://huggingface.co/hizrianraz/profile)*
