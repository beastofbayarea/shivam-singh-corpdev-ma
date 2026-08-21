# Turning execution proof into a sovereign-capital mandate

This decision connected three scales that are rarely underwritten together:

- microsecond execution behavior;
- $50 million of the firm’s proof capital; and
- a potential $500 million sovereign-capital allocation.

During my July 2016–December 2019 D. E. Shaw experience, I led the technical and commercial diligence bridge across the investor, quants, traders, hardware/infrastructure, risk, compliance, finance, and the deal committee. A benchmark could not win the mandate if it ignored live fills; a backtest could not win if it ignored controls; and a fee promise could not survive unless investment and engineering teams accepted the same evidence.

## The asset was predictable tail behavior

The CPU path looked acceptable on averages but reached eight milliseconds during market-data bursts—the exact moment prices moved fastest. Interrupts, OS queues, memory copies, and repeated GPU launches accumulated in the tail.

The proposed system used ConnectX-4 networking and GPUDirect RDMA to place market data directly in GPU memory, a persistent kernel to avoid repeated launches, and an independent FPGA gate before orders reached the exchange. [NVIDIA’s GPUDirect RDMA documentation](https://docs.nvidia.com/cuda/gpudirect-rdma/) supports the direct PCIe architecture; it does not validate these private performance figures.

Safety was independent of model intent:

- heartbeat on every processing loop;
- exchange disconnect if heartbeat stalled beyond 20 microseconds or limits broke;
- FPGA-enforced outbound order limits;
- leverage throttle when correlation fell below 0.6; and
- a retained CPU fallback.

The moat was therefore a controlled distribution with deterministic stop conditions, not a median-latency screenshot.

## Proof escalated before client exposure did

1. **Historical replay:** the 2015 Swiss-franc shock ran at 10× speed. GPU behavior stayed near 40 microseconds while the CPU path exceeded 80 milliseconds in replay.
2. **Six-week shadow:** GPU decisions were compared with production behavior without controlling capital. Recorded hedge capture was 94% versus 67% on CPU.
3. **Firm-capital proof:** $50 million ran live for four weeks.
4. **Live volatility:** independent NIC/GPU timestamps, wire taps, exchange acknowledgments, and signed logs captured referendum-shock behavior.
5. **Client mandate:** only after those gates did the $500 million allocation proceed.

The Bank of England’s [July 2016 Financial Stability Report](https://www.bankofengland.co.uk/financial-stability-report/2016/july-2016) records the market stress: a 9% fall in the sterling index between June 23 and July 1, extreme short-term volatility, lower depth, and wider spreads. It establishes the environment, not the private system result.

This proof sequence made risk asymmetric in the investor’s favor: the firm exposed its own technology and capital before asking the client to expose theirs.

## Five objections became deal conditions

**Finance:** justify $2 million of specialized hardware against recurring slippage.

**Quants:** preserve a stable Python/PyTorch research interface despite CUDA complexity.

**Infrastructure:** prove power, heat, capacity, replay, and failover for a bespoke path.

**Risk and compliance:** maintain deterministic limits independent of the strategy.

**Investor:** provide understandable, independently timed evidence without revealing proprietary code.

I synthesized those demands into one decision record. No stakeholder had to accept another team’s assertion as proof.

## The commercial structure completed the risk design

The mandate used a 1% base fee plus a 30% incentive fee only above the risk-free rate plus a 4% hurdle:

**incentive = 30% × max(0, gross eligible profit − hurdle profit)**

The base supported stewardship. Most upside depended on delivered alpha after costs and hurdle. The contract therefore turned technical diligence into aligned economics: would the execution advantage persist after hardware, operations, slippage, hurdle, and fees?

A surviving “$25 million first-year performance fees” statement cannot be reconciled because gross return, benchmark, crystallization, and base-fee treatment are missing. I exclude it.

## Mandate evidence

| Investment question | Baseline → gate → result | Measurement |
|---|---|---|
| Was stressed tail predictable? | CPU spikes to 8 ms → stable tail → 35 µs median / 40 µs p99 in cited event | Independent NIC/GPU timestamps plus exchange acknowledgments |
| Did the firm risk its own capital first? | $0 → live proof → $50M for four weeks | Capital and position ledger |
| Did execution complete intended protection? | 67% CPU shadow result → improve within limits → 94%, >4,500 hedges in cited event | Intended-order set matched to acknowledged fills |
| Was slippage bounded? | stress baseline absent → <0.5 bps → <0.5 bps | Fill price vs approved arrival benchmark |
| Was capital protected in the cited event? | client sought shock protection → avoid loss → 0.0% reported drawdown | Portfolio NAV over declared event window |
| Did evidence earn the mandate? | $0 → staged approval → $500M | Signed and funded allocation |
| Did returns clear the economics? | new mandate → hurdle + fees → 18% net reported first year | Client statement after fees |

I owned the technical/commercial thesis, proof ladder, objection synthesis, economics, committee narrative, and capital-release conditions. Quants and engineers owned models and implementation; risk/compliance owned limits; finance owned fee and cost calculations; the investor owned allocation.

The mandate was defensible because every layer exposed its failure mode: tail latency, independent controls, shadow behavior, firm capital, client capital, and fee alignment. Technical advantage became investable only after it survived realistic stress and shared risk.
