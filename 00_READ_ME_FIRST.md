# BabyFund Thailand — revised BA portfolio

**Owner:** Tankhun Luengchaicharn  
**Edition:** Portfolio submission, 11 October 2026  
**Status:** Simulated case study. A clickable Base44 mockup exists; no production app, customer funds, broker or payment partner, executed UAT, stakeholder approval, legal opinion or validated demand.

## What this case proposes

BabyFund is a **standalone coordination app** that would connect to a licensed investment partner. A guardian admits a child aged 0–10, sets multiple goals for use at or after age 20, privately invites selected people (relatives or others), and tracks a proposed gift through separate **intent → guardian decision → provider payment confirmation → partner investment confirmation → current value** states. The guest need not open a BabyFund account; this does **not** remove any identity or payer checks required by the responsible provider. The long-term investment idea is S&P 500 exposure through a suitable partner-approved vehicle. A child goal is not legal ownership; any handover at age 20 requires a separately validated process.

This is a hypothesis about reducing coordination friction in Thai families, not proof of a market gap. Dime already provides a parent-owned secondary investment account for a child and an age-20 transfer process; Kept Together supports shared child-oriented saving; K PLUS has goal-based investing. BabyFund's **proposed** point of difference is the combination of private guest invitation, no BabyFund account for the invited payer, and a visible trail to partner-confirmed investment status. Whether users want it, a provider permits it and it can earn money remain open.

Dime also offers [My Ports](https://dime.co.th/th/articles/how-to-use-my-ports) for organizing multiple goals, and [UNest](https://www.unest.co/faq) in the US offers gifting without a UNest account. Therefore neither child investing, multiple goals nor account-free gifting alone is claimed as new. The combination in the proposed Thai journey is the hypothesis to test.

## Owner decision: guardian review before guest payment

On **10 October 2026**, the owner chose **Option A** for this case study: a selected guest submits an **unpaid intent** → the guardian accepts or declines → only after acceptance may an approved provider show a payment route → the provider confirms payer and payment → the licensed partner confirms an eligible investment. A declined or expired intent receives no payment instruction. This is the selected **conceptual product sequence**, not evidence that a partner permits third-party payments or that any payment route exists. It avoids designing an unsupported hold/refund step before guardian review, but the wait for guardian action may reduce guest completion.

| Option | Sequence | Main consequence |
|---|---|---|
| A — review before payment | Intent → guardian decision → provider payment → partner investment | Less pre-decision refund complexity; guest waits for guardian |
| B — pay before review | Provider payment → guardian decision → accepted investment or provider-managed return | Requires a validated holder, payer check and return/refund route |
| C — pay guardian first | Guest pays guardian's own bank route → guardian invests with partner | Simplifies possible third-party brokerage deposit issues, but loses direct tracing unless reconciled and introduces guardian handling |

The owner selected A as the review sequence. B remains a comparison; C is a conditional fallback to investigate if direct guest funding is disallowed, not an approved route. A future licensed partner/payment provider must validate payer identity, payment acceptance, cancellation after payment, late/duplicate events, reconciliation, disputes and refunds. No document here grants BabyFund custody of money.


## Decisions added for multiple goals

- One child has one proposed partner portfolio and several goals in a planning list. Contributions join the one pooled child portfolio; goals are not separate money buckets.
- Each goal has its own target and use date **on or after the 20th birthday**. Dates may differ. The partner-confirmed child portfolio value appears once. A priority-based affordability view may subtract goals in order to show what the pooled value could cover today; this is an illustration, not reserved money.
- A guardian may set, edit or pause a **voluntary** monthly plan without a BabyFund penalty. Provider automation is a separate feasibility question.
- A goal illustration uses the one child portfolio value and that goal’s remaining months, clearly marked as a standalone scenario. A combined plan must subtract earlier planned uses to avoid counting the same money twice. Bear/base/bull are sensitivity illustrations, not probabilities of success. The owner proposes handing the whole portfolio to the adult child at age 20, subject to partner process and legal rights. Goal spending then belongs to the adult child; a transfer date and later goal dates are different events.

**Pooled model for testing:** every partner-confirmed investment has one unique event ID and changes the one child portfolio value. A payment confirmation or pending gift does not. For a simple *today* illustration, order the three targets ฿20,000, ฿50,000 and ฿100,000 against a ฿100,000 pooled value: the first two would consume ฿70,000 and leave ฿30,000 toward the third. This does not earmark assets or predict future results. The supplemental workbook now demonstrates dated contributions, three sensitivity rates and subtraction of earlier hypothetical uses. It is a fixed test example, not a production calculator or success probability.

**Partner decision gate:** before claiming any live journey, obtain evidence for legal account holder, BabyFund's own duties, approved S&P 500-linked product and suitability, third-party payer eligibility, provider payment and return route, order and valuation events, custody, withdrawal rights, age-20 transfer and data responsibilities. A failed mandatory gate blocks the live route. Option A chooses *when guardian review occurs*; it does not authorize a funding rail.

## Reading order and what changed

| File | Main revision |
|---|---|
| 01 Project Charter | Case-study status, core scope vs roadmap, proposed partner model, hypothetical targets/budget and open gates |
| 02 Stakeholder Analysis | Proposed actors, selected guest and provider responsibilities; no invented approvals |
| 03 BRD | Child goal vs legal ownership, invited gift rules, provider-dependent payment and S&P 500 scope |
| 04 FRD | Existing requirement IDs retained; separate status/data/access model, partner confirmation and conditional NFRs |
| 05 User Stories | Guest without BabyFund account, guardian review, pending/confirmed states and conditional handover |
| 06 Process Flows | Redrawn diagrams for onboarding, **owner-selected conceptual Option A**, and conditional age-20/withdrawal paths |
| 07 Use Case Diagram | Updated scope map and use cases to show provider boundary and no automatic transfer |
| 08_Wireframes_Base44_Reviewed.docx (current) | Navy/blue Word theme retained. Thirty-eight owner-supplied captures from the current Base44 demo document 13 screen groups, including active/cancelled invitation states, the account-free guest form, and distinct contribution statuses. Section 4 records visual limits and checks; screenshots do not establish live integration |
| 09 Risk Register | 25 provisional ratings, revised heat map/category totals and documented reasons for R-21–R-25 |
| 10 Gantt | Original workbook theme/formulas retained; full-delivery plan labeled hypothetical, not current portfolio hours |
| 11 UAT Test Cases | Test *design* only; added expired/forwarded invite, payer mismatch, duplicate event, partner rejection, privacy/guardian review |
| 12 Business Case Slides | Ten-slide story revised for evidence, assumptions, conditional economics and unresolved feasibility |
| 13 Calculation Evidence | Supplemental workbook with formula-driven all-goals and three-stream economics examples; not a live model |

The source 12 deliverables in the project folder were left unchanged. These files are a separate revision for review.

**Final consistency review:** The private invitation points to one child portfolio; any displayed goal is motivation, not a separate funded bucket. The timeline's B1–B14 labels represent four-week illustration blocks, not calendar months or a validated critical path. UAT contains ten detailed cases, five tabulated exception checks and seven supplemental scenario designs; none has been executed. The revised Word pages and slides were rendered and reviewed; the updated wireframe's 42 pages were exported through Word and visually checked after replacing the screenshots. Both workbooks were checked for formulas and stated examples. The guardian-review captures stop before the final on-screen note by the owner's choice. The case remains an unvalidated design for portfolio use.

The main BRD/FRD/story/UAT tables preserve their original IDs. BR-031 → FR-039 → US-21 → UAT-21/UAT-22 now traces the combined-goal example. All 25 risks have **provisional** ratings and role owners, and the heat map/category totals include R-21–R-25. Ratings are BA judgments, not observed incident rates.

## Reproducible examples, not forecasts

- The wireframe document retains a separate arithmetic example using end-of-month contributions of **฿1,500 for 240 months** from age 0 to 20, no starting balance, and constant nominal annual rates of **−2%, 5%, 8%**. Formula: `FV = P × [((1+r/12)^240 − 1)/(r/12)]`; at `r=0`, `FV=P×240`. Rounded outputs are **฿296,913 / ฿616,551 / ฿883,531**. Principal is **฿360,000**. Fees, tax, FX, inflation, cash drag and timing variation are excluded. A negative *constant* rate is just a sensitivity example, not a statistical bear case; real S&P 500 paths are volatile.
- For a child with **120** end-month payments to a chosen age-20 goal, the same ฿1,500 and rates produce **฿163,265 / ฿232,923 / ฿274,419**. The actual month count comes from the child and selected goal dates.
- Example ledger: partner-confirmed portfolio **฿100,000**; goal targets **฿20,000 + ฿50,000 + ฿100,000 = ฿170,000**. The nominal difference today is **฿70,000**. It does not prove a projected shortfall or assign value to each goal. The wireframe instead shows the single pooled value and a priority-based planning view.
- The combined-goal example starts with **฿100,000**, adds **฿500 at each month end through month 120**, then stops new contributions. Hypothetical goal uses are **฿20,000 at month 120, ฿50,000 at month 132, ฿100,000 at month 180**. For constant nominal THB rates −2% / 5% / 8%, the third goal's rounded pre-use value is **฿59,054 / ฿224,300 / ฿368,393**. Only the −2% case has a third-goal shortfall, **฿40,946**. The minimum whole-baht monthly contribution under those fixed-rate assumptions is **฿916 / ฿0 / ฿0**. The calculation is a planning sensitivity, not a probability, forecast or automatic sale. See [the workbook](13_Calculation_Evidence.xlsx) for every step.
- The revenue example uses **500 active child portfolios**, **20%** hypothetical paid conversion and **฿149/month**, giving **฿178,800 annual gross subscription sensitivity**. A **0.25% partner-level fee on ฿20m AUM** is **฿50,000** for the licensed party; an invented **20% BabyFund contractual share** would be **฿10,000** only if permitted and agreed. One **฿250,000 annual licence** is a third hypothetical line. If every entitlement and contract gate passed, the combined gross sensitivity would be **฿438,800**. Against a separate **฿1.5m synthetic annual operating-cost input**, the gap would be **฿1,061,200**. Current actual BabyFund revenue is **฿0**. These prices, conversion, fee share and costs are invented test inputs, not market evidence. UNest separately publishes a 0.25% annual management fee; the coincident 0.25% in this Thai case is still only an assumed sensitivity, not a proposed BabyFund price or a partner quote. The charter's **฿18.63m** is a separate hypothetical *delivery budget*, not annual operating cost.
- No selected S&P 500 fund/ETF, provider fee, FX mechanism, investment suitability assessment or reliable return assumption exists. The product must never imply capital protection or a guaranteed age-20 value.

## What needs validation before a credible launch case

1. **Partner and law:** legal account holder, custody, withdrawal rights, child access, age-20 handover, required licences and data/privacy roles.
2. **Payment:** whether a selected non-account guest may pay; identity/payer matching, supported bank route, expiry/revocation, duplicate/late events, holding/return/refund and reconciliation owners.
3. **Investment:** actual vehicle, eligibility/suitability, FX/fees/tax, order execution, valuation source, downturn and goal-date risk.
4. **Demand and economics:** guardian/guest interviews and usability tasks; willingness to pay; partner economics; supported market size and cost estimates.

5. **Open real-world decisions:** actual age-20 transfer rights/timing and adult spending choices, partner payment route, withdrawal terms, whether any fee share is lawful and contractually due to BabyFund, and whether guardians or B2B partners would pay. The combined-goal *illustration* now has a testable rule; it does not prescribe adult spending. A proposed one-day withdrawal delay or fee is **not an approved rule**.

These are **validation gates**, not claimed results. The UAT document contains unexecuted cases. Mock data and the owner-supplied Base44 screen captures are design artifacts, not a working integration. The current Word file, 08_Wireframes_Base44_Reviewed.docx, contains the latest supplied captures and records the prototype wording fixes. The active invitation refers to the child's pooled portfolio rather than implying a specific mutual fund. Actual token security and all partner/payment behaviour remain untested.

## Evidence and source limits

The sources below support only the specified product comparison or validation question. They do not establish market demand, an exclusive BabyFund feature, a permitted payment route, or legal approval.

| Source | What it supports in this case | What remains unknown |
|---|---|---|
| [Dime Secondary Account](https://dime.co.th/th/articles/sa-what-is-sa) | A parent-owned secondary investment account can be used for a child's future; Dime describes a process to request share transfer when the child is 20 | It does not establish that BabyFund's invited guest payment sequence is allowed or that handover is automatic |
| [Dime My Ports](https://dime.co.th/th/articles/how-to-use-my-ports) | Dime supports goal-labelled separate portfolios, up to 10 on the page checked | BabyFund's one pooled child portfolio with several *planning* goals is a proposed alternative; user preference is untested |
| [Kept Together](https://www.keptbykrungsri.com/together-savings) and [child saving use case](https://www.keptbykrungsri.com/together-savings/together-use-cases) | Shared saving and a child-oriented family example already exist; invited participants need Kept accounts | This is a savings product comparison, not proof of an equivalent S&P 500 investment or BabyFund guest flow |
| [K PLUS Goal-Based Port](https://www.kasikornbank.com/th/kplus/instruction/goal-based-port) | Goal-based investment is not a novel concept | It does not verify BabyFund's proposed payment, guest or ownership design |
| [UNest FAQ](https://www.unest.co/faq) | In the US, gifting without a UNest account and a published 0.25% annual management fee exist | US product fees and custodial rules do not determine a Thai BabyFund price, legal structure or partner entitlement |

Regulatory and payment context used as **questions for a future licensed partner**, not a legal opinion: [Bank of Thailand PromptPay overview](https://www.bot.or.th/en/financial-innovation/digital-finance/digital-payment/promptpay.html), [Thai SEC KYC/CDD guidance](https://www.sec.or.th/EN/Pages/News_Detail.aspx?Lang=EN&NewsNo=113&NewsYear=2026) and [Thai SEC mutual-fund fee disclosure update](https://www.sec.or.th/EN/Pages/News_Detail.aspx?Lang=EN&NewsNo=2&NewsYear=2026&SECID=12412). The KYC/CDD update gives same-name deposits/transfers as an audit-trail control example; it does not decide every possible guest route. The fee update concerns fund operators and selling agents; it does not grant BabyFund a management fee or licence exemption.

The earlier source list included a non-official English translation of the Securities and Exchange Act, Investor.gov educational pages and IRS Trump Account instructions without a specific claim in this portfolio that needed them. They are removed from the portfolio evidence list; removing a citation does not negate those sources.

## Owner exercise and interview practice

**Exercise (20–30 minutes):** Draw the selected Option A in five lanes (guest, guardian, BabyFund, payment provider, licensed investment partner). Add one expired invite, one payer mismatch and one partner rejection. For each step, name who owns the data and who confirms the status. Then explain why the guardian decision must precede the payment instruction and which provider assumption you would test first.

**Interview question:** “A guest can pay without a BabyFund account. How would you prevent a forwarded QR or an unmatched payer from being shown as invested, and what would you need the partner to confirm?” Answer from your diagram and UAT cases, not from a claim of actual integration.

## Owner clarifications in this revision

- Simplicity takes priority: family gifts join the child's pooled investment value. Goals are a list of desired uses, not separate funded boxes. A priority view must show remaining pooled value after earlier goals so that one baht is not counted twice.
- The owner proposes transferring the whole portfolio to the child at age 20 so the adult child can choose to hold, continue investing or redeem under actual partner terms. This is a design proposal until ownership and transfer process are validated. Ten years of holding may help a long-term saving habit but does not guarantee compound growth, reduce every form of volatility or prevent loss.
- Subscription, management fee and licensing may all be explored as **separate revenue hypotheses**. They cannot all be counted as BabyFund revenue without a payer, contractual entitlement, regulatory role, pricing and double-charge analysis.

**New exercise (15 minutes):** Starting from ฿100,000 and ฿500 a month until age 20, explain how the −2% row in the calculation workbook reaches a ฿40,946 shortfall for the third goal. State why it is wrong to add the three standalone projected balances. **Interview question:** “Who receives a management fee in this concept, and what proof would you need before showing any part of it as BabyFund revenue?”
