# Turning Execution Proof into a Sovereign-Capital Mandate

I led the technical and commercial diligence for a trading mandate from a sovereign-capital investor. I had identified that the investor needed protection during violent markets but did not want to pay fixed fees for an opaque system. I worked with the investor's team, quants, traders, infrastructure and hardware engineers, risk and compliance leaders, finance, and the deal committee.

The decision joined three scales that are usually reviewed separately: microsecond execution, $50 million of firm proof capital, and a potential $500 million client allocation. I owned the evidence bridge across all three, so the mandate could not be won by a benchmark that ignored live fills, a backtest that ignored controls, or a commercial promise that the investment and engineering teams had not accepted.

This work took place during my D. E. Shaw experience from July 2016 to December 2019. My ownership crossed an unusual boundary: determine whether a new execution platform remained predictable under stress, then decide whether that evidence justified client capital and performance-linked pricing.

## The real technical asset was the tail

The CPU path looked acceptable on ordinary averages but reached eight milliseconds during market-data bursts. The system was doing expensive work—network interrupts, operating-system queues, memory copies, and repeated GPU launches—at the moment prices moved fastest.

The proposed path used ConnectX-4 networking and GPUDirect RDMA to place market data directly into GPU memory, a persistent GPU kernel to avoid repeated launch overhead, and an independent FPGA gate before orders reached the exchange. NVIDIA's documentation supports the core architectural claim: GPUDirect RDMA creates a direct PCIe path between a network device and GPU memory, reducing CPU involvement. It does not, by itself, validate this project's latency numbers.

The safety design mattered as much as speed:

- a heartbeat updated on every processing loop;
- a heartbeat stall beyond 20 microseconds or a limit breach cut the exchange connection;
- the FPGA enforced outbound order limits independently of the model;
- correlation below 0.6 throttled leverage; and
- the CPU path remained available as a fallback.

That made the moat a controlled distribution of outcomes, not a benchmark screenshot.

## I increased proof before exposure

The validation sequence was deliberately asymmetric: the firm accepted risk before asking the client to do so.

1. **Historical stress replay:** the 2015 Swiss-franc shock was replayed at ten times speed. The GPU path stayed near 40 microseconds while the CPU path exceeded 80 milliseconds in the replay.
2. **Six-week shadow run:** GPU decisions were compared with production behavior without controlling capital. The reported capture rate was 94% versus 67% on the CPU path.
3. **Firm-capital deployment:** $50 million ran live for four weeks.
4. **Live volatility:** independent NIC/GPU timestamps, packet wire taps, exchange acknowledgements, and signed logs recorded behavior during the referendum shock.

The Bank of England's contemporaneous record establishes the external stress: between June 23 and July 1, 2016, the sterling exchange-rate index fell 9%, short-term sterling-dollar volatility reached a post-Bretton Woods high, market depth fell, and bid-offer spreads widened. Those facts explain the environment; they do not prove the private platform result.

## I translated five stakeholder objections into deal conditions

Finance challenged $2 million of specialized hardware. Quants feared CUDA complexity would slow research. Infrastructure worried about power, heat, and a bespoke failure path. Risk and Compliance required deterministic controls. The investor needed understandable evidence without proprietary source code.

I answered with one decision record: full cost versus recurring slippage, a stable Python/PyTorch research interface, replay and failover evidence, hardware-enforced limits, independent timestamps, and a staged capital plan. No group had to accept another group's assertion.

## The contract completed the product

The proposed economics were a 1% base fee plus a 30% incentive fee only above the risk-free rate plus a 4% hurdle:

`incentive fee = 30% × max(0, gross eligible profit − hurdle profit)`

That structure covered stewardship while making the largest upside conditional on delivered alpha. It also created a clean diligence question: could the execution advantage remain after hardware cost, operating cost, slippage, the hurdle, and the fee?

The surviving project notes also state “$25 million in first-year performance fees,” but they do not retain gross return, the exact risk-free benchmark, crystallization terms, or whether the figure included the 1% base fee. Because the amount cannot be reconciled from the preserved inputs, I do **not** use it as an interview claim.

## What the retained evidence supports

| Measure | Baseline | Gate | Result | Measurement |
|---|---:|---:|---:|---|
| Tail latency | CPU spikes to 8 ms in live bursts | Stable stressed tail before capital | 35 µs median / 40 µs p99 in the cited event | NIC/GPU timestamps and exchange acknowledgements |
| Firm proof capital | 0 | Firm risks capital before client | $50M | Capital and position ledger |
| Intended hedge completion | 67% CPU result in shadow comparison | Improve completion without breaking limits | 94%; more than 4,500 hedges in the cited event | Intended-order set matched to acknowledged fills |
| Execution slippage | Stress baseline not retained | Below 0.5 basis points | Below 0.5 bps | Fill price versus the approved arrival benchmark |
| Event drawdown | Client sought protection | Avoid loss during the cited shock | 0.0% reported | Portfolio NAV for the event window |
| Client allocation | 0 | Earn staged approval | $500M | Signed mandate and funded allocation |
| First-year return | New mandate | Clear the contractual hurdle | 18% net reported | Client performance statement after fees |

## Why the mandate was defensible

The platform did not win because GPUs are faster. It won because the system exposed its tail, failure modes, fallback, capital proof, and fee logic to the same decision process. The technical evidence changed the investor's risk; the contract made the manager share it.

My rule is to underwrite a technical moat where it matters most: realistic stress, independently timestamped behavior, controlled failure, client economics after all costs, and a sequence that can stop before full exposure.

### Sources and claim boundaries

| Source | Use in this reconstruction |
|---|---|
| [NVIDIA GPUDirect RDMA documentation](https://docs.nvidia.com/cuda/gpudirect-rdma/) | Supports the direct network-device-to-GPU-memory architecture and its platform constraints; not the private performance result. |
| [Bank of England Financial Stability Report, July 2016](https://www.bankofengland.co.uk/financial-stability-report/2016/july-2016) | Primary contemporaneous evidence for sterling, volatility, depth, and spread conditions around the referendum. |
| [Bank of England, liquidity determinants in the UK gilt market (2016)](https://www.bankofengland.co.uk/working-paper/2016/liquidity-determinants-in-the-uk-gilt-market) | Contemporaneous evidence that stressed liquidity and dealer conditions can materially increase execution cost. |
| [Role chronology](https://github.com/beastofbayarea/shivam-singh-corpdev-ma/blob/main/shivam-singh-corpdev-ma.pdf) | Establishes my D. E. Shaw work period; private mandate results remain attributed to the retained project record. |
