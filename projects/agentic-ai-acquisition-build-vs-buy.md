# Buying a Learning System, Not an AI Feature

I led the build-versus-buy and integration case for an AI operations company. I had identified that the buyer needed a faster way to automate supply-chain exceptions, while the target's service became uneconomic for its heaviest customers. I worked with finance, AI engineering, infrastructure and hardware teams, product leaders, independent evaluators, and the deal committee.

The proposed acquisition was $85 million. My work during my AWS experience beginning in July 2024 was to decide whether the target's poor margin revealed a broken asset or a valuable asset trapped inside a fixable architecture and pricing model.

I owned the decision as one integrated underwriting problem: price the scarce data and workflow asset, prove the model under hostile testing, make the 26-point margin expansion executable, and put a four-month integration owner behind every dependency before asking the committee to commit capital. That moved the discussion from “promising AI company” to an $85 million decision with explicit reasons to buy, build, renegotiate, or walk away.

## What we were actually considering buying

The target was growing about 60% year over year, but growth was not the moat. Its defensible assets were embedded supply-chain workflows, long-tail documents such as bills of lading and customs records, and three years of specialist corrections to real operational exceptions. An internal build could reproduce software; it could not instantly reproduce the history of how experts resolved rare cases.

I compared two counterfactuals:

| Decision factor | Build internally | Acquire and integrate |
|---|---|---|
| Time to a production offer | Estimated 18 months | Four-month integration objective |
| Workflow data | Start collecting after launch | Existing documents, exceptions, and outcomes |
| Expert feedback | No mature correction history | Three years of specialist corrections |
| Control | Full design control | Integration and inherited-dependency risk |
| Economics | Avoid purchase price; carry build and adoption risk | Pay $85M; repair current margin and pricing |
| Defensibility | Risk of a generic agent layer | Domain workflow, data, and feedback compound together |

The comparison did not make acquisition the default. It defined what the target had to prove before speed and data could justify the price.

## I wrote three walk-away conditions before the tests

First, an independent evaluation had to keep unsupported workflow output below 5%. Second, the compute and commercial redesign had to explain a credible bridge from 55% gross margin to an investable steady state. Third, the integration had to preserve customer workflows and expert feedback while adding stronger identity, safety, observability, and dependency controls.

The red team tested retrieval, orchestration, source use, and task completion—not a curated demonstration. The target reported 3.2% unsupported output against the 5% stop threshold. I treated that as a pass on one specified gate, not a claim that the product was “97% accurate.” NIST's Generative AI Profile supports that distinction: confabulation, privacy, information integrity, cybersecurity, and human control must be measured in the context of use.

The retained project record does not include the evaluation-set size or confidence interval. I would disclose that limitation in diligence and require severity slices, high-risk-task results, and regression tests before expanding autonomy.

## The margin bridge was part of underwriting, not a post-close hope

Flat-rate pricing made power users unprofitable while third-party GPU contracts kept marginal cost high. I modeled five linked changes:

1. migrate inference to lower-cost internal capacity;
2. quantize the model, reducing its footprint by roughly 40%;
3. increase concurrent reasoning chains per accelerator;
4. automate repeatable support work; and
5. replace flat pricing with a base subscription plus usage charges for compute-intensive work.

AWS guidance now describes the same engineering trade-off in operational terms: model and instance choice, quantization, concurrency, latency, throughput, utilization, and autoscaling must be benchmarked on a representative workload. I used that logic to avoid counting a cost synergy without a workload, owner, capital requirement, and acceptance test.

## The acquisition recommendation became conditional

Engineering initially saw an architecture it did not want to inherit. Finance saw a 55% margin and wanted to stop. AI Research questioned whether the product was more than a wrapper. Product leadership wanted the speed but not a year of integration disruption.

I changed the recommendation to **acquire only with the four-month integration plan funded and governed at signing**. The plan preserved the existing Kubernetes product surface, swapped the inference layer behind stable interfaces, retained the correction data, introduced source and safety gates, and moved customers to hybrid pricing without rebuilding their workflow.

That sequencing reflects a broader M&A lesson supported by current technology-deal research: product and IT value creation must be designed during diligence, because an unowned “synergy” rarely survives competing post-close priorities.

## Outcome ledger

| Measure | Baseline | Target or gate | Result | Evidence method |
|---|---:|---:|---:|---|
| Gross margin | 55% | 81% integration case | 81% | Recognized revenue less direct service and inference cost |
| Inference cost | Pre-integration index 100 | Reduce 70% | Index 30 | Cost for the representative production workload |
| Time to general availability | 18-month build estimate | Four months after close | Four months | Approved roadmap to production release |
| Unsupported-output rate | No independent accepted rate | Below 5% walk-away gate | 3.2% in diligence; 0.8% after integration | Independent task evaluation, then release-regression reporting; sample size not retained |
| Autonomous resolution | 14% | Expand only within safety gates | 72% | Eligible cases completed without specialist intervention |
| Net dollar retention | 125% | Preserve and expand retained revenue | 158% | Starting-cohort recurring revenue after churn, contraction, and expansion |

The outcome supports a strong integration case, but I keep attribution bounded. The acquired data and workflows created the starting advantage; infrastructure, pricing, safety, and customer execution created the economic result. No single lever explains the 81% margin or 158% retention on its own.

## My deal rule

I price an asset as it operates today and underwrite improvements separately. A technology acquisition becomes defensible when the scarce asset is identifiable, the failure thresholds are written before testing, the integration path is executable, and every synergy has an owner, cost, date, and measurement.

### Diligence references

- [NIST AI RMF Generative AI Profile (2024)](https://doi.org/10.6028/NIST.AI.600-1) — risk and measurement frame for independent AI diligence.
- [NIST Cybersecurity Framework 2.0 (2024)](https://doi.org/10.6028/NIST.CSWP.29) — ownership, dependency, protection, detection, response, and recovery during integration.
- [AWS SageMaker inference optimization guidance](https://docs.aws.amazon.com/sagemaker/latest/dg/model-optimize.html) — technical basis for benchmarking quantization, latency, throughput, and price.
- [Bain, technology M&A product synergies (2024)](https://www.bain.com/insights/technology-m-and-a-report-2024/) — current external evidence that product integration and customer value need investment rigor during the deal.
- [Role chronology](https://github.com/beastofbayarea/shivam-singh-corpdev-ma/blob/main/shivam-singh-corpdev-ma.pdf) — establishes my AWS work period; the target remains unnamed in the retained record.
