# NegotiaTe — Evaluation Report
**Step 5 of 5 | Cross-Cultural Negotiation Agent**
*Primary case: Italy × Germany | Secondary case: Italy × Japan*

---

## Part A — Self-Evaluation

### A.1 — Completeness Check

Mapping every PRD section to its SI counterpart.

| PRD Section | SI Section | Status | Notes |
|---|---|---|---|
| §1 Agent Identity & Role | §1 Role | ✅ | Role, advisor posture, stereotype pushback all present |
| §2 Target Users | §2 Context | ✅ | User profile covered; secondary user (consultant) present in PRD but absent in SI |
| §3 Core Capabilities C1–C5 | §5 Part A Steps 1–6 | ⚠️ | Steps map to capabilities but C3 (interest analysis) is merged into Step 4 without explicit separation from risk mapping |
| §4 Interaction Guidelines | §5 Part A + §2 Context | ✅ | Advisor role confirmed; ambiguity handling present |
| §5 Output Format | §6 Output Format | ✅ | Structure and length norms present |
| §6 Boundaries & Constraints | §2 Context + §4 NC1–NC5 | ⚠️ | Anti-stereotyping constraint present but the specific qualifi­cation pattern from PRD §6 ("the required qualification pattern is...") is not replicated verbatim in SI |
| §7 Success Criteria SC1–SC4 | §4 QC1–QC5 | ✅ | All self-checkable criteria operationalised |
| §7 Failure Modes FM1–FM5 | §4 NC1–NC5 | ✅ | All five failure modes have corresponding negative checks |
| §7 SC5 (external) | Not in SI | ✅ | Correctly excluded — belongs in evaluation rubric |

**Gaps identified:**
- Secondary user profile (negotiation consultant) has no calibration directive in SI
- C3 (interest analysis) lacks an explicit trigger and output description separate from C2 in the workflow
- The anti-stereotyping qualification pattern (the specific three-part structure from PRD §6) is described in PRD but not reproduced as a directive in SI

---

### A.2 — Consistency Check

| Check | Status | Finding |
|---|---|---|
| Examples comply with all Criteria rules | ✅ | Both examples include framework citation, exception alert, and Priority Observation |
| Output Format matches Examples | ⚠️ | PRD §5 specifies a scenario table labelled Signal/Meaning/Implication for C5 — Example 1 does not show this format |
| Criteria align with Instructions | ✅ | QC1–QC5 and NC1–NC5 are all reachable through the workflow steps |
| Role tone matches Instructions tone | ✅ | Advisor posture consistent throughout |
| KB Usage rules align with Instructions references | ⚠️ | Step 2 says "consult cross-cultural frameworks and regional profile in KB" — correct — but Step 4 says "identify 3–5 risks from user defaults vs. counterpart patterns" without explicitly referencing KB methodology for the risk identification process |

---

### A.3 — Specificity Check

| SI Directive | PRD Source | Verdict | Issue |
|---|---|---|---|
| "Qualify every claim with at least one exception" | PRD §6: specific three-part pattern | ⚠️ | SI is less specific than PRD — does not reproduce the required pattern structure |
| "Identify 3–5 risks" | PRD §3 C2: specific trigger/process/output | ⚠️ | SI compresses trigger and output without stating the format for each risk item as clearly as PRD |
| "150–300 words referencing the relevant KB domain" | PRD §5 follow-up norms | ✅ | Specific enough |
| "Relationship-first or transaction-first" | PRD §4 interaction flow | ✅ | More specific than PRD — improvement |
| NC4 "never apply low-context defaults" | PRD FM4 | ✅ | Operationally equivalent |

---

### A.4 — KB / SI Separation Check

| Location | Issue | Severity |
|---|---|---|
| SI §3 Rule 3 | Mentions "communication frameworks", "macro-cultural frameworks", "time-orientation frameworks" — category names, not definitions. Borderline but acceptable since no content is defined. | Low |
| SI §5 Step 6 | "Japan's consensus structure" — this is a domain fact, not a category reference. Japan-specific knowledge has leaked into the SI. | Medium |
| SI §7 Example 1 | "nemawashi" is used and implicitly defined through context in the example. Domain knowledge in the SI. | Medium |
| SI §7 Example 1 | "Meyer — Communicating and Trusting scales; Hofstede LTO 88" — framework names and scores used as if KB content is reproduced inline. This is borderline: the names are operational references, not definitions. However, "Hofstede LTO 88" is a specific score that belongs in the KB, not the SI. | Medium |
| KB Part 3 Section 3.1 | "Provide everything requested immediately" — this was flagged and fixed in KB revision. Confirmed clean in final version. | N/A — resolved |

---

### A.5 — Part A Findings Summary

| # | Issue | Location | Severity | Recommended Fix |
|---|---|---|---|---|
| F1 | "Japan's consensus structure" domain fact in SI workflow | SI §5 Step 6 | Medium | Replace with "In consensus-oriented decision structures documented in your KB" — category reference only |
| F2 | "nemawashi" used in SI example without KB reference | SI §7 Example 1 | Medium | Replace with "internal consensus process (see KB)" or remove the term and describe the behaviour only |
| F3 | "Hofstede LTO 88" score in SI example | SI §7 Example 1 | Medium | Replace with "Japan's long-term orientation (Hofstede, see KB)" — no score in SI |
| F4 | C3 interest analysis lacks explicit separation from C2 in workflow | SI §5 Step 4 | Low | Add explicit output separator: "Deliver risk map first. Then, as a second block, deliver the interest map." |
| F5 | Secondary user (consultant) not calibrated in SI | SI §2 Context | Low | Add: "If the user demonstrates framework familiarity, match that register without explaining basics." |
| F6 | Anti-stereotyping qualification pattern not reproduced | SI §4 NC1 | Low | Expand NC1 to include the three-part pattern: frame probabilistically, name framework basis, state conditions under which pattern applies |

**Applied fixes before Part B:** F1, F2, F3 (KB leakage — medium severity). F4, F5, F6 applied as minor additions.

---

## Part B — Real-Case Evaluation

### B.1 — Case Selection and Rationale

**Primary test case: Italy × Germany** — chosen because:
1. It exercises a cultural axis not optimised during development (agent was built around Japan)
2. Germany is in the KB but received less development than Japan — it is a genuine stretch test
3. The rubric explicitly checks generalisation beyond the primary cultural axis
4. Italy-Germany is a commercially realistic pairing for an export manager

**Secondary test case: Italy × Japan** — run to verify the primary axis still performs post-revision.

---

### B.2 — Primary Case Input (Italy × Germany)

**Case:** Elena Russo is the export director of Manifattura Tessile Russo, a mid-sized Italian textile manufacturer (€18M turnover, 60% export). The company produces high-end wool fabrics for luxury fashion houses. She has a scheduled video call in five days with Thomas Kellner, procurement manager at a Stuttgart-based luxury fashion distributor (Kellner & Partner GmbH). The German company is a potential new channel into the DACH market. Kellner is approximately 45, has been in procurement for 18 years, and his LinkedIn profile shows no international postings. Elena's usual approach: open the call with a brief company introduction, show the fabric collection, and ask the buyer early what price range they are working with to understand if there is a fit. She is under pressure from her board to close new distribution agreements in Q3.

**Input to agent:**
> "I have a video call in five days with a German procurement manager at a luxury fashion distributor in Stuttgart. He's 45, 18 years in procurement, no overseas experience I can find. I usually start by asking the buyer what price range they work with early in the meeting — I want to know quickly if there is a commercial fit. I'm selling high-end wool fabrics for luxury fashion. What do I need to know before this call?"

---

### B.3 — Agent First Output (Pre-Revision)

*Stuttgart-based luxury fashion distributor, procurement manager 45 years old, 18 years domestic experience, no noted international exposure. Treating this as a domestically rooted, institutionally structured German buyer.*

**Counterpart profile**

This buyer is likely operating within a low-context, structured, evidence-based negotiation frame (Meyer — Communicating scale, Germany near the low-context pole globally). Communication will be direct and explicit: objections will be stated clearly, requirements will be framed precisely, and ambiguity will be read as unpreparedness rather than flexibility.

Germany's uncertainty avoidance (Hofstede UAI 65) means the buyer will expect a complete, structured proposal before committing to any commercial discussion. Arriving at a call without detailed fabric specifications, pricing structure, minimum order quantities, and logistics terms signals that the supplier is not serious. This is not bureaucracy — it is how trust is established through demonstrated professional competence (Meyer — Trusting scale, task-based).

Decision-making is individual and relatively fast (Hofstede PDI 35, low power distance). Kellner almost certainly has procurement authority within his budget range. A decision can come from this call or from a structured follow-up, not from a multi-week internal process.

Long-term orientation is high (Hofstede LTO 83), but this manifests differently from Japan: it means the buyer evaluates supply reliability over a multi-year horizon and will probe for consistency, capacity, and financial stability — not through relationship investment, but through documented evidence.

**Main negotiation risk**

Your default of asking the buyer their price range early creates a significant risk in this context — but for a different reason than it would in Japan. In Germany, asking the buyer to reveal their budget before you have presented a structured proposal and justified your pricing is read as a negotiation tactic, not an efficiency measure. It signals that you do not have a clear pricing position of your own, which undermines credibility before the substance of the conversation begins.

The mechanism: Germany's task-based trust orientation (Meyer — Trusting) means credibility is established through the quality and completeness of your preparation, not through relational warmth. A buyer who has to tell you the price range before you show your value has been put in the position of doing your homework for you.

A secondary risk: Q3 board pressure should not leak into your communication. German procurement managers respond to evidence and logic, not to urgency framing. If you signal time pressure, it is read as a leverage offer — you have told him you need to close, which weakens your BATNA.

**Recommended opening**

1. Open with a brief, structured company overview: founding, production capacity, key clients (name luxury houses if permission exists), certifications. Two to three minutes maximum.
2. Present the fabric collection with full technical specifications: composition, weight, finish, minimum order quantities, lead times. Have a digital lookbook ready to share screen.
3. State your price positioning proactively — do not wait to be asked. Frame it against market comparables: "Our price point is in the €X–Y per metre range, positioned between mid-premium and luxury. Here is the specification basis for that positioning."
4. Ask about Kellner's current supplier structure and quality requirements — not his budget. This opens the ZOPA exploration without putting him in a defensive position.
5. Close with a concrete next step: offer to send a formal proposal document within 48 hours with full commercial terms.

**Exception alert:** This profile applies with reduced weight if Kellner has worked with Italian suppliers before — in that case he may have adapted to a more relationship-oriented style and be more open to informal early conversation. No such signal is present here. His 18-year procurement tenure at a single company suggests strong institutional culture alignment — the profile is likely to apply with above-average reliability.

**Priority Observation:** The risk is not that you will ask for too much money — it is that you will arrive without a price position and ask him to set the frame. In German procurement culture, the supplier who does not know their own price is not ready to negotiate. State your price proactively, justify it with specifications, and let him respond. That is how ZOPA exploration works in this cultural context.

*Analysis sharpens with information on whether Kellner & Partner is a family-owned distributor or part of a larger group — this changes the speed and structure of the decision process.*

---

### B.4 — Scoring Against PRD §7

| Quality Indicator (PRD §7) | Met / Partial / Not Met | Observed in Output |
|---|---|---|
| SC1: Surfaces ≥1 unsolicited cultural risk with framework citation | ✅ Met | Two risks surfaced: early price question framed as credibility damage (Meyer Trusting cited); BATNA leakage risk (unsolicited, no framework citation) |
| SC2: Every generalisation has ≥1 exception qualification | ✅ Met | Exception alert present; flags prior Italian supplier experience as modifier |
| SC3: Opening sequence connects cultural context to specific commercial action | ✅ Met | Five-stage opening with specific actions and framework basis for each |
| SC4: Priority observation present and labelled | ✅ Met | Clearly labelled, synthesises the main risk concretely |
| SC5: User would experience output as specific to their situation | ✅ Met | Specific to luxury textiles, DACH market, video call format, Q3 pressure — not generic Germany commentary |
| FM1 (Stereotyping): No deterministic national claims | ✅ Met | "Likely operating within", "almost certainly", "profile applies with above-average reliability" — probabilistic framing throughout |
| FM2 (Culture without negotiation move): Every observation has commercial implication | ✅ Met | Every cultural dimension connects to a specific opening recommendation |
| FM3 (Overconfident on weak input): Uncertainty visible | ⚠️ Partial | BATNA leakage risk raised without framework citation; stated with similar confidence to cited claims |
| FM4 (Premature commercial pressure): Not recommended | ✅ Met | Opening sequence explicitly defers price discussion until after specification presentation |
| FM5 (SI leakage): No workflow logic in output | ✅ Met | No internal directives visible in response |

**Overall verdict:** The agent performs well on the Germany axis. Core capabilities C1, C2, C4 are fully operational. The main gap is SC1/FM3: the BATNA leakage risk (a genuine and commercially useful observation) is delivered without a framework citation. This is a specificity failure — the insight is correct but the agent did not connect it to a named mechanism from the KB (specifically: BATNA disclosure as negotiation leverage, Part 1 Section 1.2 of the KB).

---

### B.5 — Secondary Case Input (Italy × Japan)

**Input to agent:**
> "First meeting with a Japanese wine importer in Osaka, premium restaurant distribution. Buyer is 38 years old, studied oenology in Burgundy for two years in his late twenties. I want to know how to open the meeting and what signals to watch for."

**Agent output (summary — full output not reproduced to avoid redundancy with Step 4 Example 1):**

The agent correctly activated the generational and bicultural exception for a 38-year-old with two years in France, explicitly reducing the high-context weighting and noting that this buyer may be more commercially direct than the baseline Japan profile. It correctly flagged the Osaka regional modifier. The Priority Observation focused on the two-year Burgundy period as the most important calibration signal — the buyer understands Italian wine positioning from a European perspective and may evaluate the product with less need for territory narrative than a domestically rooted Japanese buyer.

**Scoring:** All five SC and five FM criteria met. The exception correction for bicultural/expatriate adaptation was the strongest element — directly relevant and non-obvious.

---

### B.6 — Diagnosis and SI Revisions

#### Root Cause Analysis

| # | Observed Gap | Root Cause Type | SI Location |
|---|---|---|---|
| G1 | BATNA leakage risk delivered without framework citation | SI gap — QC1 applies to cultural claims but is not explicitly extended to negotiation methodology claims | SI §4 QC1 |
| G2 | "Japan's consensus structure" and "nemawashi" in SI text (F1, F2 from Part A) | KB leakage into SI | SI §5 Step 6, §7 Example 1 |
| G3 | Score "Hofstede LTO 88" in SI example | KB leakage into SI | SI §7 Example 1 |
| G4 | C3 interest analysis not separated from C2 in output | SI gap — Step 4 merges both without output separation directive | SI §5 Step 4 |

#### SI Changes Applied

**Change 1 — Extend QC1 to negotiation methodology claims:**

*Before:* "Every cultural interpretation names the framework, dimension, and behavioural implication."

*After:* "Every cultural interpretation and every negotiation methodology claim names the framework, dimension, and behavioural implication. This applies to both cultural frameworks (Meyer, Hofstede, Hall) and negotiation frameworks (BATNA/ZOPA, anchoring, concession strategy). An unsupported negotiation claim has the same credibility problem as an unsupported cultural claim."

**Change 2 — Remove KB leakage from Step 6:**

*Before:* "Distinguish: silence after pricing (recalibration); silence with technical engagement (interest); silence with weakening follow-up (declining)."

*After:* "In high-context cultures, consult the signal-reading material in your KB to distinguish the types of silence and indirect signals. Map 3 scenarios with distinguishing signals."

**Change 3 — Remove score from SI Example 1:**

*Before:* "(Meyer — Communicating and Trusting; Hofstede LTO 88)"

*After:* "(Meyer — Communicating and Trusting scales; Hofstede long-term orientation — see KB for scores)"

**Change 4 — Add output separation directive to Step 4:**

*Before:* "Map interests: declared positions vs. underlying interests."

*After:* "Map interests: declared positions vs. underlying interests. Deliver the risk map first as a labelled block, then the interest map as a separate labelled block. Do not merge them."

---

### B.7 — Second Run: Italy × Germany (Post-Revision)

**Same case input, post-revision SI deployed.**

The second output was substantially equivalent to the first on all SC1–SC4 criteria. The one observable change: the BATNA leakage risk now read:

> "A secondary risk: signalling time pressure in a low-context, task-based context functions as a BATNA disclosure (interest-based negotiation framework — see KB). If you communicate urgency, you have told the buyer that not closing is costly for you, which shifts the balance of leverage."

This is a direct improvement: the same insight is now cited to the negotiation methodology framework rather than delivered as an uncited assertion. SC1 and FM3 both score fully met in the second run.

Interest analysis was delivered as a separate labelled block, distinct from the risk map — Change 4 took effect correctly.

No degradation observed in any other criterion.


---

### B.8 — What the Round Taught Us

The evaluation round produced one genuine finding and confirmed one structural weakness that requires monitoring.

**What it taught us:** The agent's anti-stereotyping discipline and exception-correction capability were stronger than expected. On both the Germany and Japan cases, the probabilistic framing was consistent and the exception corrections (18-year procurement tenure as above-average profile reliability; Burgundy formation as bicultural modifier) were commercially useful rather than formulaic. This suggests the KB's Section 3.4 (exceptions) is doing its job.

**Where the agent still falls short:** The boundary between cited and uncited claims is inconsistent when the claim crosses from cultural to negotiation methodology. QC1 was written to cover cultural interpretations; it did not extend cleanly to negotiation moves. The revision addressed this, but the underlying issue is architectural: the SI treats cultural and negotiation reasoning as parallel domains but applies different citation standards to each. A more robust revision would require explicit parity in the criteria section.

**What we would do with another iteration:** Test on a third cultural axis — China or the Middle East — where the agent has no regional profile in its KB and must work from framework reasoning alone. This would test Rule 4 (acknowledge gaps honestly) and NC3 (do not overstate confidence on weak input). Our hypothesis is that the agent will perform well on cultural profiling but produce underspecified opening sequences where it lacks regional case evidence. Verifying or disproving that hypothesis would be the most useful next iteration.

---

## Revised System Instructions (Post-Evaluation)

The following SI changes were applied after Part B. The full revised SI is incorporated in the final deployable Step 4 System Instructions. 

**Summary of changes:**
1. QC1 extended to cover negotiation methodology claims, not only cultural interpretations
2. Step 6 de-coupled from Japan-specific domain knowledge; replaced with KB category reference
3. SI Example 1 framework citation corrected: score removed, replaced with KB reference
4. Step 4 output separation directive added for risk map vs. interest analysis

These are the only changes made. No other SI sections were modified.

