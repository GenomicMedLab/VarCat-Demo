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
**Evidence** is the information used to support or refute an assertion.

Evidence is handled in two steps:

1. **Curation**:
   - VarCat pulls in evidence automatically from a variety of sources where possible. Users may optionally add additional evidence from other sources or edit the VarCat-curated evidence if desired.
2. **Application**:
   - Curated evidence must be applied to an assertion by giving it a **score** that tells VarCat the _strength_ and _directionality_ of its impact:
      - **Directionality**: Whether the Evidence _supports_ or _refutes_ the statement the Assertion is attempting to make
      - **Strength**: How _confident_ we are that this evidence supports that conclusion

#### Shared Evidence
Evidence for a variant is **shared** across all of that variant's assessments to reduce duplicative curation efforts.

Because of this, editing evidence can affect other assessments. In most cases, evidence should be added or unapplied, not edited or deleted.

## Evidence Line
Evidence items of the same type are grouped together under a single **evidence line**. All items grouped under a given evidence line are evaluated as one and are applied **under a single score**.


## Assessment Statuses
Assessments move through a lifecycle of the following statuses:

1. `Pending`
2. `Active`
3. `Awaiting Review`
4. `In Review`
5. `Reviewed`

An assessment can return to `Pending` if it needs to be worked again.

## Quick-Reference Glossary
| Term | Meaning |
| ---- | ------- |
| _Assessment_ | A review of one variant and one disease pairing. |
| _Assertion_ | One conclusion within an assessment. |
| _Evidence_ | Information used to support or refute an assertion. |
| _Evidence Line_ | A set of related evidence items scored together. |
| _Assessment Status_ | The current stage of the assessment workflow. |
