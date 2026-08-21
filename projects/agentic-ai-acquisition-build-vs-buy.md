# Reframing an $85 Million Agentic AI Acquisition

I led this build-versus-buy and integration work during my [AWS experience beginning in July 2024](https://github.com/beastofbayarea/shivam-singh-corpdev-ma/blob/main/shivam-singh-corpdev-ma.pdf).

The acquisition target had strong growth, proprietary workflow data, and years of expert corrections. It also had a serious economic problem: flat-rate pricing and third-party infrastructure made its heaviest users unprofitable. Engineering and Finance initially saw that margin profile as a reason to stop the deal.

I saw a different diligence question. Was the asset structurally weak, or was a valuable asset trapped inside a fixable cost and commercial model?

## I separated the moat from the operating model

I compared an internal build and an acquisition across time to market, proprietary data, accumulated expert feedback, technical quality, execution risk, integration cost, and defensibility. Building offered control, but it would take an estimated 18 months and would begin without the target's correction data. Acquiring could compress that timeline, provided the underlying system passed independent tests and the post-close economics were executable.

I therefore made the recommendation conditional. The target had to clear three gates:

1. The system's unsupported-output rate had to remain below a pre-agreed 5% walk-away threshold.
2. The infrastructure and pricing changes had to produce a credible gross-margin bridge.
3. The integration plan had to preserve product velocity while introducing stronger platform, safety, and governance controls.

## Technical diligence had an explicit stop condition

I commissioned an independent red-team of the retrieval and orchestration stack rather than accept a curated demonstration. NIST's Generative AI Profile shaped the evaluation frame: confabulation, information integrity, privacy, cybersecurity, human oversight, and measurement all had to be considered together.

The target measured 3.2% against the 5% hallucination threshold. Passing did not mean the system was risk-free. It meant the observed behavior was within the boundary we had defined before seeing the result, and the residual risk could be governed through product and operational controls.

## I built value creation into the deal thesis

The margin bridge combined infrastructure migration, model quantization, concurrency improvements, support automation, and hybrid usage pricing. That model projected a 70% reduction in inference cost and an increase in gross margin from 55% to 81%.

The integration plan ran across four months in four connected lanes:

- migrate compute without redesigning the customer experience;
- introduce model and safety controls with observable release gates;
- preserve the workflow data and expert-feedback loop that made the asset defensible; and
- replace flat pricing with a structure that aligned revenue to costly usage.

NIST's Cybersecurity Framework 2.0 informed the governance and supply-chain work, including named ownership, dependency risk, protection, detection, response, and recovery.

## The recommendation changed—but remained conditional

I changed the recommendation from “stop” to “acquire with conditions.” The resulting plan accelerated general availability from an estimated 18 months to four. Inference cost fell 70%, gross margin reached 81%, autonomous resolution increased from 14% to 72%, and net dollar retention reached 158%.

## What I believe made the decision defensible

I did not ask the investment team to overlook poor current margins. I showed which part of the value came from the asset, which part depended on post-close execution, what evidence would invalidate the thesis, and who would own each integration outcome.

That is how I approach technology acquisitions: price the asset as it exists, underwrite the improvements separately, and refuse to count a synergy until it has an owner, sequence, cost, and measurable release condition.

## External foundations

These sources supplied the primary diligence and governance methodology. My resume is linked only to establish employment chronology.

| Source | How I applied it |
|---|---|
| [NIST — Generative AI Profile (2024)](https://doi.org/10.6028/NIST.AI.600-1) | I used its risk categories and measurement guidance to structure independent red-team diligence and residual-risk decisions. |
| [NIST — Cybersecurity Framework 2.0 (2024)](https://doi.org/10.6028/NIST.CSWP.29) | I used its govern-identify-protect-detect-respond-recover functions to frame integration ownership and supply-chain risk. |
