# Pharmacy DRP Screening & Classification Guide

**The classification standard behind [`Pharmacy-README.md`](Pharmacy-README.md) — how a drug-related problem gets identified, classified, and documented at the point of dispensing.**

## 1. What counts as a DRP

A drug-related problem (DRP) is any event or circumstance involving drug therapy that actually or potentially interferes with a desired health outcome — the working definition used by the Pharmaceutical Care Network Europe (PCNE), whose classification (V9.1) this framework is built on.

## 2. PCNE's core distinction: problem vs. cause

PCNE's classification is built around a distinction most informal systems collapse into one: it separates *the problem* (what went wrong, clinically) from *the cause* (why it happened). A single cause — a prescribing slip, a missed allergy check — is logged separately from its clinical consequence. This framework follows the same split.

### Problem domains (PCNE's 3 primary domains)

| Domain | Covers |
|---|---|
| Treatment Safety | The therapy as prescribed poses a safety risk — an interaction, an allergy conflict, a dose inappropriate for the patient's physiology |
| Treatment Effectiveness | The therapy isn't achieving what it should — an untreated indication, a dose or duration that won't work |
| Other | Doesn't cleanly fit either domain — unclear complaints, patient-related circumstances like a refill pattern suggesting non-adherence |

### Cause categories (this framework's working set)

Not every DRP a dispensing screen catches needs PCNE's full 9-domain cause taxonomy at the level of detail a single-pharmacy log uses day to day, so this framework uses a working set of the causes that come up most often at the point of dispensing:

- **Drug Interaction** — two prescribed drugs interact
- **Drug-Allergy Conflict** — a prescribed drug conflicts with a documented allergy
- **Inappropriate Dose** — dose doesn't match age, weight, renal/hepatic function, or pregnancy status
- **Therapeutic Duplication** — two drugs from the same class, often from different prescribers
- **Untreated Indication** — a guideline-recommended therapy is missing
- **Inappropriate Duration** — course length doesn't match the indication
- **Dispensing/Logistics Error** — a picking, labeling, or patient-identification error caught before handover
- **Patient-Related** — adherence patterns or other patient-side circumstances

## 3. Severity

- **Critical** — could cause real patient harm if not caught: interactions with a serious clinical consequence, allergy conflicts, dosing errors in a vulnerable population (renal impairment, pediatrics, pregnancy), a near-miss on the wrong patient.
- **Moderate** — a real gap, but lower immediate risk: therapeutic duplication without an acute interaction, a duration or indication gap, a labeling error caught before it reached the patient.

## 4. Screening steps, in order

1. **Medication list review** — reconcile against what the patient is actually taking, not just what's on this one prescription.
2. **Allergy check** — cross-reference against documented allergies before anything else.
3. **Interaction check** — screen the full current medication list, not just the new item.
4. **Dose-appropriateness check** — age, weight, renal/hepatic function, pregnancy status.
5. **Duplication check** — same drug or same class already on the list.
6. **Indication check** — is there a guideline-recommended therapy that's missing, not just a problem with what's present.

Any "No" at steps 2–6 gets flagged before dispensing, not noted for later — the checklist in [`Pharmacy-DRP-Log.xlsx`](Pharmacy-DRP-Log.xlsx) exists specifically so this happens at the counter, not after the patient has left.

## 5. Intervention & documentation

- Every identified DRP gets an intervention (contact the prescriber, counsel the patient, or both) and an outcome, logged in the same record as the problem — not just noted separately.
- A "Pending" outcome means the loop isn't closed yet; it stays open until it is, rather than being logged once and forgotten.

---

*Companion files: [`Pharmacy-README.md`](Pharmacy-README.md) for the full case study, `Pharmacy-DRP-Log.xlsx` for the screening log this guide is derived from.*
