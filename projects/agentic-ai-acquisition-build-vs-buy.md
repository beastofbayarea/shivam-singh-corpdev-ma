# Buying a learning system, not an AI feature

## Investment committee decision

**Proposed consideration:** $85 million  
**Alternative:** build internally over an estimated 18 months  
**Recommendation:** acquire only if independent model diligence, an executable 26-point gross-margin bridge, and a funded four-month integration plan all cleared before commitment.

Beginning in my July 2024 AWS experience, the build-versus-buy analysis and integration underwriting fell to me across Finance, AI Engineering, Infrastructure/Hardware, Product, independent evaluators, and the deal committee.

The target was growing roughly 60% year over year, but heavy users were economically unattractive. The committee initially saw either a promising AI company or a 55%-margin asset to reject. I reframed the question: **was the target structurally broken, or did it own a scarce learning system trapped inside fixable compute and pricing choices?**

## What the $85 million would actually buy

The software surface was reproducible. The scarce assets were not:

- embedded supply-chain exception workflows;
- long-tail operational documents, including bills of lading and customs records;
- three years of specialist corrections linked to real outcomes; and
- customer behavior inside a difficult, recurring operational job.

An internal build offered full design control and no purchase price, but it would begin collecting documents, exceptions, and expert feedback only after launch. Acquisition offered production workflows and accumulated correction history, while importing architecture, dependency, and integration risk.

The target therefore had to prove that its domain data and feedback loop would compound faster than a clean internal build—not merely that its demo was ahead.

## I wrote the reasons to walk away before the evidence arrived

### 1. Model-behavior gate

Unsupported workflow output had to remain below 5% in an independent, representative evaluation. The red team tested retrieval, orchestration, source use, and end-task completion rather than curated prompts.

The target recorded 3.2%. I treated that as one gate cleared, not “96.8% accuracy.” Sample size and confidence interval are absent from the retained record, so I required severity slices, high-risk-task results, and regression tests before expanding autonomy.

[NIST’s Generative AI Profile](https://doi.org/10.6028/NIST.AI.600-1) informed the broader risk perimeter: confabulation, privacy, information integrity, security, and human control had to be assessed in the actual workflow.

### 2. Economic gate

Gross margin had to move from 55% to an underwritten 81% steady state through named, measurable levers:

1. migrate inference from costly third-party GPU contracts to lower-cost internal capacity;
2. quantize the model, reducing footprint roughly 40%;
3. increase concurrent reasoning chains per accelerator;
4. automate repeatable support work; and
5. replace flat pricing with a base subscription plus usage charges for compute-intensive work.

Every lever carried workload, capital, owner, implementation date, and acceptance test. [AWS model-optimization guidance](https://docs.aws.amazon.com/sagemaker/latest/dg/model-optimize.html) supports benchmarking quantization, throughput, utilization, latency, and price on representative workloads; it does not prove this deal’s synergy.

### 3. Integration gate

The buyer had to preserve the target’s customer workflows and correction data while strengthening identity, source attribution, safety, observability, and dependency control.

Engineering did not want to inherit the stack. Product wanted speed without a year of disruption. I built a four-month sequence that kept the Kubernetes product surface stable, swapped inference behind controlled interfaces, introduced source/safety gates, retained the feedback history, and migrated customers to hybrid pricing without forcing a workflow rebuild.

I made that plan a signing condition with funded owners. An integration aspiration written after close would not support the valuation.

## Why the conditional recommendation won alignment

Finance could see the margin bridge rather than accept “AI scale economics.” Research could see independent task behavior rather than wrapper rhetoric. Engineering could see the interfaces and inherited dependencies it would own. Product could see what remained stable for customers. The committee could compare acquire, build, renegotiate, and walk away on the same evidence.

Current technology-M&A research similarly argues that product and IT value creation must be designed in diligence, not left as an unowned post-close synergy. I used that principle to make integration part of underwriting.

## Outcome against the thesis

| Investment assumption | Baseline → gate/target → recorded result | Verification |
|---|---|---|
| Gross margin | 55% → 81% integration case → 81% | Recognized revenue less direct service and inference cost |
| Inference economics | cost index 100 → -70% → 30 | Representative production workload at equivalent quality/latency |
| Time advantage | 18-month build estimate → 4-month post-close GA → 4 months | Signed roadmap to generally available integrated product |
| Unsupported output | no accepted independent rate → <5% → 3.2% diligence, 0.8% post-integration | Independent task set, then release regression; sample size not retained |
| Autonomous resolution | 14% → expand only inside safety gates → 72% | Eligible cases completed without specialist intervention |
| Net dollar retention | 125% → preserve and expand cohort revenue → 158% | Starting recurring-revenue cohort after churn, contraction, and expansion |

The 81% margin and 158% NDR cannot be attributed to one lever. Acquired workflow/data created the starting advantage; compute, pricing, controls, integration, and customer execution determined realization.

The investment thesis, definition of the scarce asset, build counterfactual, prewritten walk-away gates, technical/economic diligence synthesis, conditional recommendation, integration value plan, and committee record were my transaction work product.

My deal rule is simple: price the asset as it operates today; underwrite improvements separately. A technology acquisition deserves capital only when the scarce asset is identifiable, failure conditions precede the test, and every synergy has an owner, cost, date, and measurable path through integration.
