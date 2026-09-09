# Concepts to Know

## Overview
VarCat assists users in evaluating somatic variant/disease pairings by curating evidence to support conclusions about oncogenicity and, when needed, therapeutic, diagnostic, and/or prognostic significance.

## Core Terms
### Assessment
An **assessment** is a review of one variant/disease pairing.

### Assertion
An **assertion** is one conclusion within an assessment.

Every assessment contains one or more assertions that analyze different aspects of the pairing according to the following standardized guidelines: 

- **[ClinGen/CGC/VICC Oncogenicity Standard Operating Procedures](https://cancervariants.org/research/standards/onc_path_sop/):**
   - Oncogenicity Classification*
- **[AMP/ASCO/CAP Guidelines](https://pubmed.ncbi.nlm.nih.gov/27993330/):**
   - Therapeutic Response
   - Diagnostic Inclusion/Exclusion
   - Prognostic Outcome Prediction

\*An Oncogenicity Classification assertion is **required** on every assessment; all other assertions are optional.

### Evidence
**Evidence** is the information used to support or refute an assertion. It is handled in two steps:

1. **Curation**:
   - VarCat pulls in evidence automatically from a variety of sources where possible. Users may optionally add additional evidence from other sources or edit the VarCat-curated evidence if desired.
2. **Application**:
   - Curated evidence must be **applied** to an assertion by giving it a score that tells VarCat the _strength_ and _directionality_ of its impact:
      - **Directionality**: Whether the Evidence _supports_ or _refutes_ the statement the Assertion is attempting to make
      - **Strength**: How _confident_ we are that this evidence supports that conclusion
   - Similar evidence is applied together and evaluated as one - see [Evidence Line](#evidence-line) below.

#### A Note on Applying Evidence: `Not Applied`/`Not Applicable` and `Not Assessed`
Evidence can be applied a variety of different ways, depending on its type; however, most evidence will have the option of being applied as `Not Assessed`, and all evidence can be set to `Not Applied`:
   - `Not Assessed`: Indicates that this evidence was **not evaluated**. It has no impact on the Assertion's overall score, either positively or negatively.
   - `Not Applied`/`Not Applicable`: Indicates that this evidence was determined to be **irrelevant** to the Assertion. It also has no impact on the Assertion's overall score.

#### Shared Evidence
Evidence for a variant is **shared** across all of that variant's assessments to reduce duplicative curation efforts.

Because of this, editing evidence can affect other assessments. In most cases, evidence should be added or unapplied, not edited or deleted. Evidence is **locked** (i.e., unable to be edited) after an assessment on which it's been applied is set to `Reviewed` (see [Assessment Status](#assessment-status) below).

### Evidence Line
Evidence items of the same type are grouped together under a single **evidence line**. All items grouped under a given evidence line are evaluated as one and are applied **under a single score**.


### Assessment Status
Assessments move through a lifecycle of the following statuses:

1. `Pending`: Assessment has not yet been completed.
2. `Active`: Assessment is actively being filled out.
3. `Awaiting Review`: Assessment is complete, but awaiting expert review and final sign-off.
4. `In Review`: Assessment is being reviewed by a subject matter expert (e.g., Clinical Director or similar)
5. `Reviewed`: Assessment has received sign-off from the Reviewer and is now finalized. 

An assessment can return to `Pending` if it needs to be worked again.

## Quick-Reference Glossary
| Term | Meaning |
| ---- | ------- |
| _Assessment_ | A review of one variant and one disease pairing. |
| _Assertion_ | One conclusion within an assessment. |
| _Evidence_ | Information used to support or refute an assertion. |
| _Evidence Line_ | A set of related evidence items scored together. |
| _Assessment Status_ | The current stage of the assessment workflow. |

## Anatomy of an Assessment

![Assessment layout](/documentation/images/assessment-anatomy.png)

1. **Header**: identifies the variant/disease pairing.
2. **Status Section**: shows the assessment's current [status](#assessment-status), checkout information, and status history. Use this section to:
    - _Move_ the assessment to the next or previous status
    - _Overtake_ an active assessment from another user
    - _Review_ the assessment's status history, including _who_ previously checked out the assessment and _when_
3. **Summary Modal**: lists the assessment's assertions (left) and displays a summary of the selected assertion (right), including its:
    - _Classification_: The current conclusion drawn by this assertion
    - _Score_: The current strength of support the applied evidence has for this conclusion
    - _Applied Evidence_: A summary list of the evidence currently contributing to that result
4. **Evidence Tabs**: contain the evidence for each assertion type.
5. **Table of contents sidebar**: allows quick navigation to the various sections of the assessment.
6. **Info Tab**: An dynamically-updating informational sidebar with additional explanations about VarCat and the content of the current tab.