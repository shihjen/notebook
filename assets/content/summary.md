# AI Research Summary Report

*Generated on: 1/1/2026, 2:07:30 AM*

---

## GamiBench: Evaluating Spatial Reasoning and 2D-to-3D Planning Capabilities of MLLMs with Origami Folding Tasks
**Authors:** Ryan Spencer, Roey Yaari, Ritvik Vemavarapu, Joyce Yang, Steven Ngo, Utkarsh Sharma

**Link:** [Read Paper](https://arxiv.org/abs/2512.22207)

### Summary
**GamiBench – A Spatial‑Reasoning Benchmark for Multimodal LLMs**

**Problem & Motivation**  
- Existing multimodal large language models (MLLMs) excel at perception and instruction‑following but lack robust *spatial reasoning*—the capacity to mentally track and manipulate objects across multiple views and over time.  
- Most current benchmarks only evaluate static images or final outputs, ignoring the sequential, viewpoint‑dependent nature of spatial tasks.

**Core Contribution**  
- **GamiBench** – a new benchmark built around origami‑inspired folding tasks that require 2D‑to‑3D reasoning.  
- The benchmark probes the *entire* reasoning pipeline rather than just final predictions.

**Dataset**  
- 372 crease patterns: 186 *regular* (foldable) and 186 *impossible* (non‑foldable) 2D shapes.  
- Each pattern paired with its 3D folded shape.  
- Six distinct viewpoints generated for each shape, spanning three VQA sub‑tasks:  
  1. Predicting the 3‑D fold configuration.  
  2. Determining which viewpoints are valid.  
  3. Detecting impossible patterns.

**Evaluation Focus**  
- **Cross‑view consistency** – models must agree across viewpoints.  
- **Physical feasibility** – detecting impossible folds.  
- **Intermediate step interpretation** – reasoning about the folding process itself.

**New Diagnostic Metrics**  
- **Viewpoint Consistency (VC)** – measures agreement across different views.  
- **Impossible Fold Selection Rate (IFSR)** – evaluates how well models identify impossible patterns.

**Findings**  
- Even state‑of‑the‑art MLLMs (GPT‑5, Gemini‑2.5‑Pro) struggle with single‑step spatial understanding when evaluated on GamiBench.  
- The benchmark exposes gaps in models’ geometric intuition and sequential reasoning abilities.

**Impact**  
- Provides a standardized, challenging framework for testing and improving geometric and spatial reasoning in multimodal LLMs.  
- The dataset and evaluation code are publicly available: https://github.com/stvngo/GamiBench.

*Processed at: 2026-01-01T08:53:24.322+08:00*

---

## Toward Equitable Recovery: A Fairness-Aware AI Framework for Prioritizing Post-Flood Aid in Bangladesh
**Authors:** Farjana Yesmin, Romana Akter

**Link:** [Read Paper](https://arxiv.org/abs/2512.22210)

### Summary
**Summary**

The paper introduces a fairness‑aware AI system designed to improve post‑flood aid allocation in Bangladesh, a nation that frequently faces devastating floods. Using 2022 flood data that impacted 7.2 million people and caused $405.5 million in damage, the authors build an **adversarial debiasing model** that predicts flood vulnerability while explicitly removing bias against historically marginalized districts and rural areas.

Key technical contributions:

1. **Gradient‑reversal layer** (adapted from healthcare AI) forces the model to learn bias‑invariant representations.
2. The model is trained on data from 87 upazilas in 11 districts.

Performance highlights:

- **Statistical parity difference** reduced by **41.6 %**.
- **Regional fairness gaps** shrank by **43.2 %**.
- **Predictive accuracy** remains strong (R² = 0.784 vs baseline 0.811).

Outcome: The system generates actionable priority rankings that allocate aid based on genuine need rather than historical allocation patterns, demonstrating that algorithmic fairness methods can be effectively applied to humanitarian decision‑making.

*Processed at: 2026-01-01T08:53:24.322+08:00*

---

