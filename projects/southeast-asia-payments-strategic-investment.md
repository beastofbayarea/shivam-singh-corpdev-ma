# Redirecting a wallet bet toward Southeast Asia’s payment rails

The original proposal put $50 million behind a visible consumer wallet. I recommended abandoning it.

Customer-acquisition cost had tripled since 2020, retention without subsidy was below 40%, take rate was near 0.5%, and more than 50 regional wallets were competing for the same attention. The scarce asset was not another front end. It was interoperability among wallets, banks, merchant acquirers, and national schemes.

During my Rakuten internship, I led the strategic-investment case across the investment committee, fintech leadership, founders, local regulators and counsel, product/engineering, and Japanese travelers. I redirected the thesis from buying users repeatedly to owning a minority position in the rails that connected them.

## The target: a B2B aggregator

The aggregator earned a reported 1.5–2.0% cross-border take rate and offered one integration through which Rakuten Pay could gain utility across selected corridors.

The strategic and financial theses were kept independent:

- **Financial:** corridor volume, take rate, operating leverage, cash requirement, downside valuation.
- **Strategic:** enabled acceptance for existing Rakuten users, integration cost/timing, payment success, and travel-triggered usage.

Either case had to stand without borrowing value from the other.

I helped structure a 15% minority investment with delivery milestones and future-rights protection. After valuation rose, the position captured too little upside. I documented the lesson: pro-rata rights or warrant coverage should have been non-negotiable, even at the cost of a longer process.

## I underwrote corridors as options, not flags on a map

Every market received its own diligence:

- license and scheme participation;
- merchant coverage and endpoint quality;
- settlement, FX, fraud, dispute, and reversal economics;
- technical interface and reconciliation;
- existing Rakuten traveler demand; and
- local counsel/regulator evidence.

A strong company did not make every corridor launchable.

I initially accepted a six-month Vietnam assumption based too heavily on target counsel. Settlement requirements blocked launch for 12 months—a six-month miss. I reported it to the committee as a diligence error, separated enterprise value from corridor permission, required independent local review, and staged further integration spend behind licensing evidence.

Thailand and Singapore advanced earlier because their scheme and partner paths were clearer. Vietnam remained a separately governed option rather than contaminating a regional average.

The [World Bank Fast Payments Toolkit](https://fastpayments.worldbank.org/sites/default/files/2021-11/Fast%20Payment%20Flagship_Final_Nov%201.pdf) supports this system view across interoperability, QR, APIs, governance, fraud, disputes, and settlement. Primary central-bank sources also distinguish person-to-person linkages such as [PromptPay–PayNow](https://www.bot.or.th/en/news-and-media/news/news-20210429.html) from merchant-QR connections. I did not treat one as proof of the other.

## The integration was a transaction workstream

The aggregator exposed REST APIs; Rakuten’s Japanese payments core used ISO 8583 and local accounting conventions. I brought Tokyo engineers to Singapore for a three-day working session to settle:

**authentication → message/currency mapping → ISO 8583 authorization → scheme routing → merchant confirmation → reversal → settlement → reconciliation**

Idempotency, payment success, timeout behavior, duplicates, chargebacks, support, and ledger reconciliation were release gates. An API 200 response was not an end-to-end payment.

[PCI DSS 4.0](https://www.pcisecuritystandards.org/standards/pci-dss/) supplied the payment-data control baseline across access, logging, change, and continuous validation.

## Distribution used an existing customer moment

A Japanese customer booking regional travel could learn before departure that Rakuten Pay worked on an enabled rail. This aligned activation with a real payment need and avoided recreating the wallet’s paid-subsidy model.

## Investment outcome ledger

| Underwriting dimension | Baseline → objective → recorded result | Evidence |
|---|---|---|
| Capital direction | $50M wallet proposal → own a defensible layer → 15% infrastructure position | Approved transaction |
| Consumer economics avoided | CAC 3× 2020, retention <40%, take rate ~0.5% → stop subsidy dependence → B2B take rate 1.5–2.0% | Cohort and revenue diligence |
| Acceptance surface | no integrated cross-border reach → selected-corridor utility → >5M reported QR points | Enabled endpoints, not 5M active transacting merchants |
| Vietnam schedule | 6 months → approval-gated launch → blocked 12 months | Corridor plan vs regulatory milestone |
| Company economics | loss-making → breakeven → EBITDA breakeven in 14 months | Management accounts |
| Investment value | 1.0× entry book value → preserve/grow → ~1.5× | Portfolio valuation, not realized cash return |

I owned the thesis reversal, target/layer choice, minority structure, corridor model, regulatory escalation, integration dependency, distribution logic, valuation monitoring, and committee account.

The corporate-development lesson was sharper than “infrastructure beats apps.” A regional network, a permitted corridor, a working integration, and defensible minority rights are separate assets. I now price and gate them separately so the visible size of a network cannot hide where strategic value is unable to launch.
