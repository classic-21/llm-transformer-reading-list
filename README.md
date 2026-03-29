# LLM & Transformer Internals — A Curated Reading List
### Free Preview: Transformer Foundations

*Curated by Priyanshu Singh*

---

What this is: A carefully filtered collection of the best articles, papers, books, and videos for understanding how LLMs and transformers work from the inside — the architecture, the inference mechanics, the training pipelines, and how the field has evolved. Every entry was evaluated individually. Many were left out.

**Who this is for:** Engineers, researchers, and serious learners who want to go beyond using LLMs to actually understanding them.

**What this is not:** Prompt engineering, agent design, LLMOps, or application-layer tutorials. The focus is the internals.

---

## Tier System

**⭐ Essential** — foundational, high-signal, read regardless of experience level  
**✅ Excellent** — strong depth, worth your time once you have the foundations

---

## Section 1: Transformer Foundations
*The core mechanism — start here*

This is where every serious study of LLM internals begins. The transformer architecture, introduced in 2017, is the foundation of every model discussed in the full guide. These four resources approach it from different angles — visual, geometric, historical, and intuitive — and together they give a complete picture of what attention is and why it matters.

---

### The Illustrated Transformer
**Jay Alammar · Article**  
⭐ Essential · Start here

This is the most widely used visual introduction to the transformer architecture in existence. Alammar walks through the encoder-decoder structure, multi-head attention, and positional encoding with custom illustrations that make the flow of information through the model genuinely clear. It has been translated into over a dozen languages and cited by learners across every level of the field. The reason it holds up years later is that it explains the architecture as a system — not just the math, but the shape of how data moves. If you read only one thing from this entire list first, make it this.

🔗 https://jalammar.github.io/illustrated-transformer/

*Pairs with: The 3Blue1Brown video below, which covers the same ideas through a different lens.*

---

### Attention in Transformers, Visually Explained
**3Blue1Brown (Grant Sanderson) · Video**  
⭐ Essential · Watch second

Grant Sanderson approaches the Q/K/V attention mechanism geometrically — how meaning gets encoded in high-dimensional space, and why the dot-product scoring of queries against keys is actually doing something meaningful. The animation quality is exceptional, and the geometric framing builds a different kind of intuition than Alammar's diagram-based approach. The two resources complement each other: Alammar shows you the architecture, Sanderson shows you why the math behind it makes sense.

🔗 https://www.youtube.com/watch?v=eMlx5fFNoYc

*Prerequisite: Basic familiarity with vectors and matrix multiplication is helpful but not required.*

---

### Attention? Attention!
**Lilian Weng · Article**  
⭐ Essential · Read third

Lilian Weng was Head of Safety Research at OpenAI when she wrote this — and the rigor shows. This article traces the full intellectual history of attention: from the encoder-decoder bottleneck problem in early sequence models, through the invention of the attention mechanism as a fix for it, and into the transformer. Reading this in sequence after Alammar and 3Blue1Brown gives you the historical and theoretical grounding that explains why attention was invented in the first place, not just how it works.

🔗 https://lilianweng.github.io/posts/2018-06-24-attention/

*Prerequisite: Comfort with the Alammar article. Some exposure to RNNs is helpful for appreciating the problem that attention solves.*

---

### Some Intuition on Attention and the Transformer
**Eugene Yan · Article**  
⭐ Essential · Read fourth

Explicitly written for people who have already read the original "Attention Is All You Need" paper and want to go deeper. Yan builds intuition around two things most introductions gloss over: why the fixed-size context vector in older encoder-decoder models was a fundamental bottleneck, and how attention's ability to let the decoder attend to the full input sequence changes what the model can represent. The writing is clear and the diagrams are well-chosen. It sits at the right level of depth — more demanding than Alammar, less exhaustive than Weng.

🔗 https://eugeneyan.com/writing/attention/

*Prerequisite: The Alammar article. Even better if you've skimmed "Attention Is All You Need."*

---

**Section reading path:** Alammar → 3Blue1Brown → Weng → Yan. Each resource adds a layer on top of the previous one. Do not skip the order here — the later entries assume the earlier ones.

---

## What's in the Full Guide

This free section covers the foundations.

The full guide covers 8 more sections beyond this one, going deep into how models are trained, how inference actually works, the foundational papers the field is built on, and the best books for systematic understanding.

Each section follows the same structure, with annotations, reading order, and pairing notes throughout. Reading paths by experience level are included — whether you're starting from scratch or already familiar with the basics.

35+ resources in total. Every one personally evaluated. Many were left out.

---

**Full guide:** [classicpsy.gumroad.com/l/llm-transformer-internals](https://classicpsy.gumroad.com/l/llm-transformer-internals) · $9

Questions or suggestions: psyadav7743@gmail.com

© 2026 Priyanshu Singh. Licensed under CC BY-NC-ND 4.0. Free to share with attribution. Not for commercial use or modification.
---

*Last reviewed: March 2026*
