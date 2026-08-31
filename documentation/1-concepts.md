# Concepts to Know

## Overview
The Variation Categorizer (VarCat) is designed to help with somatic variant prioritization and interpretation by utilizing the ClinGen/CGC/VICC Oncogenicity SOP and AMP/ASCO/CAP guidelines to evaluate **oncogenicity**, **therapeutic response**, **prognostic evidence**, and **diagnostic evidence** for various variant/disease pairings. It is intended to assess SNVs and less complex forms of variation in accordance with the ClinGen/CGC/VICC Oncogenicity guidelines.


## Assessments and Assertions
VarCat is organized around `Assessments` that evaluate specific variant-disease pairings. Each assessment contains several `Assertions` that analyze different aspects of the pairing using the following standardized guidelines: 

- **[ClinGen/CGC/VICC Oncogenicity Guidelines](https://cancervariants.org/research/standards/onc_path_sop/):**
    - Oncogenicity Classification
- **[AMP/ASCO/CAP Guidelines](https://pubmed.ncbi.nlm.nih.gov/27993330/):**
    - Therapeutic Response
    - Diagnostic Inclusion/Exclusion
    - Prognostic Outcome Prediction

For example, an Oncogenicity Classification Assertion for an Assessment of **TP53 Asp281His** + **Rhabdomyosarcoma** might be: _"TP53 p.Asp281His is classified **likely oncogenic** in Rhabdomyosarcoma."_ A Diagnostic Assertion for the same variant/disease pairing might be: _"TP53 supports a **strong clinical significance** classification as an **inclusion** criterion for Rhabdomyosarcoma."_

Each assessment _must_ contain an Oncogenicity assertion, and may optionally include one or more AMP/ASCO/CAP assertions as well.


## Evidence
Each Assertion on an Assessment is supported by `Evidence`. Adding Evidence to an Assertion is done in two steps: first, Evidence is _curated_, then it is _applied_:

### Curating Evidence
VarCat automatically pulls in Evidence from a variety of sources for all of an Assessment's Assertions. Assessors can also add their own evidence if they wish to include data from sources outside of those that VarCat sources on its own (TODO: See link here for tutorial).

Evidence related to a given variant is **shared** across all of that variant's Assessments. This means that evidence only has to be curated once, eliminating the need for duplicate work!

### Applying Evidence
Once Evidence is curated, it needs to be _applied_ to the Assertion it supports/refutes. This gives the evidence a **score** that tells VarCat HOW the evidence impacts the Assertion, both in terms of _directionality_ and  _strength_:

- a) **Directionality**: Whether the Evidence supports or refutes the statement the Assertion is attempting to make, and
- b) **Strength**: How confident we are that this evidence supports that conclusion

Individual Evidence items are not applied on their own; instead, items of the same type are grouped together. All Evidence items under a given grouping are evaluated as one and are applied to the Assertion **under a single score**.

For example, one group of Evidence may report a set of gnomAD allele frequency data about TP53 p.Asp281His to provide _moderate_ evidence _supporting_ a proposition that it causes Rhabdomyosarcoma.

VarCat automatically applies Evidence for Oncogenicity Assertions, but Assessors may change if/how these items are applied if they wish. 


### ⚠️ Editing/Deleting Evidence
Because Evidence is shared across Assessments, editing Evidence items is generally **not advised**, as edits may have unintended consequences on other Assessments that have already applied the Evidence. Therefore, this functionality is largely unavailable, with a few exceptions. For instance, in some places this problem is circumvented by allowing "edits" that create fresh copies of the original item containing the new updates.

For the same reason, deletion of Evidence items is not enabled.


## Assessment Status Lifecycle
Assessments progress through a "lifecycle" of statuses, as follows:

1. `Pending`: The Assessment has not yet been performed.
2. `Active`: The Assessment is currently in the process of being edited.
3. `Awaiting Review`: The Assessment has been cursorily completed, but requires review and sign-off from a subject matter expert.
4. `In Review`: Expert review of the Assessment is currently underway.
5. `Reviewed`: The Assessment has received expert sign-off and is finalized.

Assessments may transition from `Reviewed` back to `Pending` to re-start the cycle; e.g., for workflows that require periodic re-review of Assessments to ensure Evidence is kept up-to-date.


## Quick-Reference Glossary
| _Term_ | _Definition_ |
| ---- | ---------- |
| **Assessment** | An evaluation of a variant-disease pairing. |
| **Assertion** | An appraisal of one aspect of a given variant-disease pairing. Each Assessment contains an _Oncogenicity Classification,_  plus one or more of the following Assertions: _Therapeutic Response,_ _Diagnostic evaluation,_ and/or _Prognostic evaluation._ |
| **Evidence Grouping** | A group of related **Evidence** items that are evaluated together to support or refute an **Assertion.** |
| **Evidence** | A data-supported fact. |
| **Assessment Status** | Indicates what stage the Assessment is in within its curation lifecycle |