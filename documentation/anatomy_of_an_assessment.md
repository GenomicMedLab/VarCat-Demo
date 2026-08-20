# Anatomy of an Assessment
The following is a breakdown of the various sections of an variant/disease pairing Assessment page:

![](/documentation/images/assessment-anatomy.png)


## 1. Assessment Header

![alt text](/documentation/images/header.png)

The header displays the variant/disease pairing being evaluated in this Assessment.


## 2. Status Section

![alt text](/documentation/images/status-section.png)

Assessments progress through a "lifecycle" of statuses, as follows:

- `Pending`: The Assessment has not yet been performed.
- `Active`: The Assessment is currently in the process of being edited.
- `Awaiting Review`: The Assessment has been cursorily completed, but requires review and sign-off from a subject matter expert.
- `In Review`: Expert review of the Assessment is currently underway.
- `Reviewed`: The Assessment has received expert sign-off and is finalized.

Assessments may transition from `Reviewed` back to `Pending` to re-start the cycle; e.g., for workflows that require periodic re-review of Assessments to ensure evidence is kept up-to-date.

The Status section displays the Assessment's current status, including which user (if any) currently has the Assessment checked out. It also allows Assessors to advance to the next stage or go back to the previous one.

In addition, you may view the Assessment's status history, including _which_ stages it has been through, _when_ it transitioned between stages, and _who_ performed each stage.


## 3. Summary Modal

![alt text](/documentation/images/summary-modal.png)
<figcaption><i>Summary modal, with the "Weak Supporting" Applied Evidence section expanded</i></figcaption>
<br/>
The summary modal displays a tabbed list of all of the Assessment's Assertions (left-hand side), with some high-level info about the currently-selected Assertion (right-hand side), including its:

- **Classification**: _"TP53 p.Asp281His is classified **likely oncogenic** in Rhabdomyosarcoma"_
- **Score**: As displayed by the sliding scale, the Oncogenicity Assertion above is scored as a `9` on a scale of `-7` to `10`, which falls in the category of `Likely Oncogenic`. This score is calculated based on the scores of the evidence that has been applied to it (see "Evidence Tabs" below for more details)
- **Applied Evidence**: An expandable list of all the evidence supporting this Assertion's classification. For Oncogenicity Assertions, these items are grouped and sorted by **strength**. All other Assertions group evidence by **type**. Click on a grouping to expand the section and view all evidence items it contains.


## 4. Evidence Tabs


Beneath the summary modal are tab displaying all of the evidence to support each Assertion as required by the [ClinGen/CGC/VICC Oncogenicity Standard Operating Procedure](https://cancervariants.org/research/standards/onc_path_sop/) (for Oncogenicity Assertions) or the [AMP/ASCO/CAP](https://pubmed.ncbi.nlm.nih.gov/27993330/) guidelines (for all other Assertions).

The Evidence Tabs look different depending on the type of Assertion you're viewing, as explained below:

### Oncogenicity Classification Tab

![alt text](/documentation/images/evidence-section.png)

Here, Evidence is grouped into sections by type, and each section receives a **code** to denote its significance, as well as a **score** that indicates the _strength_ and _direction_ of the data as it applies to this Assertion. 

For example, take a look at the above section titled "Effect on Protein Product". Notice that VarCat has automatically selected a code of `Not Applicable`, and a score of `0` for this section. However, Assessors can change both of these using the dropdown menus if desired. Assessors may also manually add evidence of their own to this section via the "Add Evidence" button. 

The Oncogenicity Assertion's overall score (displayed in the summary modal above) is the **sum total** of each individual sections' scores. 

### Other Assertion Evidence Tabs

![alt text](/documentation/images/evidence-tab-diagnostic.png)

All other Assertions display their evidence in tables, with tabs showing evidence for the **specific variant** associated with this assessment as well as evidence more broadly relevant to this variant's **gene**. 

Evidence from these tables can be applied to the current Assertion using the dropdowns in the `Apply As` column. To edit evidence, select the pencil icon in the `Edit` column*. To add new evidence, use the "Add Evidence" button in the upper right-hand corner of the tab. 

> ⚠️ **\* CAUTION:** Editing evidence may impact other assessments. Learn more about editing evidence HERE [#TODO].

The overall score for a non-oncogenic Assertion is equivalent to that of the **highest-ranked evidence applied to it**.

### Previous Classifications Tab

![alt text](/documentation/images/prev-classifications.png)

Unlike the other tabs, The Previous Classifications tab does _NOT_ display evidence that can be applied to an Assertion on this Assessment. Instead, it displays how this variant has been classified _when paired with other diseases_, or how _other variants on the same gene_ have been classified on other Assessments. This may serve as a useful reference for Assessors as they complete Assertions on the current Assessment.

## 5. Table of Contents Sidebar

![alt text](/documentation/images/table-of-contents-sidebar.png)

The Table of Contents sidebar allows quick navigation to any section/sub-section of the Assessment.