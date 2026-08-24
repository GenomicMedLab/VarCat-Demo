# Concepts to Know


## Assessments and Assertions
VarCat is organized around `Assessments` that evaluate specific variant-disease pairings. Each assessment contains several `Assertions` that analyze different aspects of the pairing using the following standardized guidelines: 

- **ClinGen/CGC/VICC Oncogenicity Guidelines:**
    - Oncogenicity Classification
- **AMP/ASCO/CAP Guidelines:**
    - Therapeutic Response
    - Diagnostic Inclusion/Exclusion
    - Prognostic Outcome Prediction

For example, an Oncogenicity Classification Assertion for an Assessment of **TP53 Asp281His** + **Rhabdomyosarcoma** might be: _"TP53 p.Asp281His is classified **likely oncogenic** in Rhabdomyosarcoma."_ A Diagnostic Assertion for the same variant/disease pairing might be: _"TP53 supports a **strong clinical significance** classification as an **inclusion** criterion for Rhabdomyosarcoma."_

Each assessment _must_ contain an Oncogenicity assertion, and may optionally include one or more AMP/ASCO/CAP assertions as well.


## Evidence
Each Assertion is supported by `Evidence`. Evidence items of the same type are grouped together. All Evidence items under a given grouping are evaluated together, and the group's overall _strength_ and _directionality_ are applied to the Assertion under one score. For example, one group of Evidence may report a set of gnomAD allele frequency data about TP53 p.Asp281His to provide _moderate_ evidence _supporting_ a proposition that it causes Rhabdomyosarcoma.

VarCat automatically pulls in evidence from a variety of sources and computes an automated score for each relevant Evidence grouping. Assessors can manually apply/un-apply evidence as needed, as well as adjust the weight and directionality for these scores. They can also add their own evidence if they wish to include data from sources outside of those that VarCat pulls in on its own.

<!-- ### ⚠️ Editing Evidence -->




## Assessment Status
Assessments progress through a "lifecycle" of statuses, as follows:

1. `Pending`: The Assessment has not yet been performed.
2. `Active`: The Assessment is currently in the process of being edited.
3. `Awaiting Review`: The Assessment has been cursorily completed, but requires review and sign-off from a subject matter expert.
4. `In Review`: Expert review of the Assessment is currently underway.
5. `Reviewed`: The Assessment has received expert sign-off and is finalized.

Assessments may transition from `Reviewed` back to `Pending` to re-start the cycle; e.g., for workflows that require periodic re-review of Assessments to ensure evidence is kept up-to-date.


## Glossary
| _Term_ | _Definition_ |
| ---- | ---------- |
| **Assessment** | An evaluation of a variant-disease pairing. |
| **Assertion** | An appraisal of one aspect of a given variant-disease pairing. Each Assessment contains an _Oncogenicity Classification,_  plus one or more of the following Assertions: _Therapeutic Response,_ _Diagnostic evaluation,_ and/or _Prognostic evaluation._ |
| **Evidence Grouping** | A group of related **Evidence** items that together support or refute an **Assertion.** |
| **Evidence** | A proven fact. |