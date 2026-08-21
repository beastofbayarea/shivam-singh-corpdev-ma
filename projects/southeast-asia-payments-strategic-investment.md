# Redirecting a Wallet Bet Toward Southeast Asia's Payment Rails

I led a strategic-investment case for cross-border payments in Southeast Asia. I had identified that another consumer wallet would keep paying to win the same travelers, while banks, wallets, and merchants still lacked a dependable way to work together. I worked with the investment committee, FinTech leaders, founders, local regulators and counsel, product and engineering teams, and Japanese customers traveling in the region.

## The thesis changed before the cheque

The original $50 million thesis favored a visible consumer wallet. The operating evidence was deteriorating: customer-acquisition cost had tripled since 2020, retention without subsidy was below 40%, and take rates were near 0.5%. The region also contained more than 50 wallets, which made consumer attention abundant to compete for and interoperability scarce to own.

I redirected the case toward a B2B aggregator connecting wallets, banks, merchant acquirers, and national payment schemes. Its cross-border economics supported a reported 1.5%–2.0% take rate, and an integration could add regional utility to customers Rakuten already had rather than buy them again.

That conclusion matched the public direction of the market. The World Bank's Fast Payments Toolkit treats access, interoperability, QR standards, APIs, governance, fraud, disputes, and settlement as one implementation system. Central-bank projects were also linking national rails: Thailand and Singapore launched PromptPay–PayNow real-time transfers in 2021, while separate merchant-QR linkages connected schemes such as PromptPay, NETS, DuitNow, and VietQR.

I kept those products distinct in the diligence. A person-to-person transfer linkage is not automatically merchant QR acceptance.

## The transaction had to create two independent forms of value

I supported a 15% minority investment in the aggregator. The financial thesis was sticky B2B volume, higher take rate, and operating leverage. The strategic thesis was a bridge from Rakuten Pay into regional acceptance for Japanese travelers.

I tracked the two cases separately:

| Financial case | Strategic case |
|---|---|
| Corridor revenue and take rate | Enabled acceptance for existing users |
| EBITDA path and cash need | Integration cost and launch timing |
| Downside valuation | Customer usage and payment success |
| Minority protections and follow-on rights | Data, scheme, security, and support obligations |

The deal included delivery milestones and future-rights protection. In retrospect, the 15% position captured too little upside after the target's valuation increased; I would insist on pro-rata rights or warrant coverage even if negotiation took longer.

## Every corridor was its own product

I scored markets on license status, scheme participation, merchant coverage, settlement and foreign-exchange economics, fraud and dispute rules, technical interfaces, and existing Rakuten travel demand. A strong company did not make an unlicensed corridor launchable.

I initially accepted a six-month Vietnam launch assumption based too heavily on the target's counsel. State Bank of Vietnam settlement requirements blocked launch for 12 months. That was a six-month schedule miss against the original plan, and I documented it to the committee as a diligence error rather than hiding it in a regional average.

I then separated company-level value from corridor-level permission, required independent local regulatory review, and staged integration spending behind licensing evidence. Thailand and Singapore moved earlier because their scheme and partner paths were clearer; Vietnam remained a separately governed option.

## The technical bridge was part of the deal thesis

The aggregator exposed modern REST APIs. Rakuten's Japanese payment core used ISO 8583 messages and local accounting conventions. I brought Tokyo engineers to Singapore for a three-day working session and aligned the message translation, authorization, idempotency, settlement, reversal, and reconciliation boundaries.

The path was explicit:

`Rakuten Pay request → API authentication → message and currency mapping → ISO 8583 authorization → regional scheme → merchant confirmation → settlement and reconciliation`

Security gates followed PCI DSS 4.0 principles for payment-account data, access, logging, change control, and continuous validation. Commercial launch also required payment-success, reversal, settlement, and support readiness; an API response alone was not an end-to-end payment.

## Distribution followed an existing customer need

Instead of buying local wallet users, the team used owned travel signals. A Japanese customer booking a trip could learn before departure that Rakuten Pay worked on the enabled regional rails. This aligned activation with a real need and avoided reproducing the consumer wallet's subsidy problem.

## Results and boundaries

| Measure | Baseline | Objective | Result | Evidence basis |
|---|---:|---:|---:|---|
| Capital thesis | $50M consumer-wallet proposal | Move capital to a more defensible layer | 15% infrastructure position | Approved transaction record |
| Consumer economics | CAC 3× 2020 level; retention <40%; take rate ~0.5% | Avoid recurring subsidized acquisition | B2B take rate 1.5%–2.0% | Diligence cohort and revenue analysis |
| Regional acceptance | No integrated cross-border reach from the product | Enable one integration across selected corridors | More than 5M reported QR acceptance points | Aggregator's enabled-endpoint reporting; not claimed as 5M active transacting merchants |
| Vietnam timing | Six-month assumption | Launch after approval | Blocked for 12 months | Corridor plan versus regulatory milestone record |
| B2B economics | Pre-scale loss position | Reach breakeven | EBITDA breakeven in 14 months | Portfolio-company management accounts |
| Investment value | Entry book value 1.0× | Preserve and grow | About 1.5× book value | Portfolio valuation record, not a realized cash return |

## The corporate-development lesson

A regional network and a launchable corridor are different assets. I now underwrite the company, each regulatory route, the integration, the distribution advantage, and the minority rights separately. A strategic investment is ready only when both the financial return case and the product advantage can survive on their own evidence.

### Market and implementation evidence

- [World Bank Fast Payments Toolkit (2021)](https://fastpayments.worldbank.org/sites/default/files/2021-11/Fast%20Payment%20Flagship_Final_Nov%201.pdf) — system-level diligence across interoperability, QR, APIs, governance, risk, and implementation.
- [Bank of Thailand and MAS, PromptPay–PayNow linkage (2021)](https://www.bot.or.th/en/news-and-media/news/news-20210429.html) — primary evidence for the bilateral real-time transfer rail and its limits.
- [Bank of Thailand, cross-border payment map](https://www.bot.or.th/en/financial-innovation/digital-finance/digital-payment/cross-border-payment.html) — distinguishes real-time remittance from merchant QR linkages, including Thailand–Vietnam.
- [Bank Negara Malaysia and MAS, DuitNow–NETS QR linkage (2023)](https://www.bnm.gov.my/-/qrcode-connectivity-my-sg) — primary example of cross-border merchant QR interoperability.
- [PCI Security Standards Council, PCI DSS 4.0](https://www.pcisecuritystandards.org/standards/pci-dss/) — payment-data control baseline.
- [Role chronology](https://github.com/beastofbayarea/shivam-singh-corpdev-ma/blob/main/shivam-singh-corpdev-ma.pdf) — establishes my Rakuten work period from June to December 2023.
