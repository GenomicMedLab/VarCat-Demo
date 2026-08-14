# Tutorial: How To Complete An Assessment

[DELETE] /17-7673779-C-G/ncit:C3359

## Overview
The Variation Categorizer (VarCat) is designed to help with somatic variant prioritization and interpretation by utilizing the ClinGen/CGC/VICC Oncogenicity SOP and AMP/ASCO/CAP guidelines to evaluate **oncogenicity**, **therapeutic response**, **prognostic evidence**, and **diagnostic evidence** for various variant/disease pairings. It is intended to assess SNVs and less complex forms of variation in accordance with the ClinGen/CGC/VICC Oncogenicity guidelines.

The following is a guide outlining how to utilize VarCat to complete such an evaluation.

## 1. Open an Assessment
From the homepage, open an Assessment by either:

  - a) Selecting an Assessment from the list, or 
  - b) Entering a variant/disease pairing of your choosing in the selection form above the table. 

![alt text](/documentation/images/landing-page.png)

## 2. Change the Assessment's Status to `Active`:

In order to edit an Assessment, you must set its status to `Active` via the status button in the upper-right hand corner. Depending on the Assessment's current status, you may need to cycle through several stages before reaching "Active:"

![alt text](/documentation/images/start-assessment.png)

Only one person may edit an Assessment at a time. If your Assessment is already active, but is checked out to someone else, you will need to overtake the Assessment from them:

![alt text](/documentation/images/overtake-assessment.jpg)


## 3. Examine & Edit the Auto-Computed Oncogenicity Assertion:

VarCat automatically pulls in data from a variety of sources, and use this evidence to auto-generate an initial Oncogenicity Assertion for the Assessment. Evaluate each section to add evidence you've curated yourself, change the section's **code**, and/or update the section's **score** as applicable.

![alt text](/documentation/images/edit-onco-evidence-scode.png)
<figcaption><i>Editing a section's evidence code</i></figcaption>


## 4. [Optional] Add Additional Assertions:
In addition to the required Oncogenicity Assertion, all Assessments may optionally include one or more additional Assertions following the [AMP/ASCO/CAP](https://pubmed.ncbi.nlm.nih.gov/27993330/) guidelines.

To view an Assertion that's already been created, click on the corresponding tab in the Summary Modal:

![alt text](/documentation/images/summary-tab-diagnostic-inclusion.png)

To add or edit the Assertion's evidence, or to create a new Assertion, click on the appropriate tab beneath the summary modal:

![alt text](/documentation/images/evidence-tab-diagnostic-click.png)

Here you'll see a list of evidence that's relevant to this Assessment's **variant**, or its **gene.** Toggle back and forth between these views using the toggle at the top of the chart:

![alt text](/documentation/images/case-control-gene.png)

![alt text](/documentation/images/case-control-variant.png)

VarCat will automatically pull in evidence from a variety of sources that will auto-populate these tables where possible. You may also manually curate evidence by selecting the "Add Evidence" button in to the upper right of the table, and filling in the curation form:

![alt text](/documentation/images/add-evidence-click.png)

![alt text](/documentation/images/add-evidence-modal.png)

Once you've selected or created the evidence you'd like to use, apply it to the Assertion by using the dropdown in the "Apply As" column (if not already applied):

![alt text](/documentation/images/apply-evidence.png)

Notice that the Summary Modal updates to display the newly-applied evidence, grouped by **type** (note: you may need to refresh the page). The Assertion's **score** and **classification** will also update based on the evidence you apply and how you apply it.

![alt text](/documentation/images/summary-modal-updated.png)

To manually upgrade or downgrade all evidence in a given category, use the dropdown options in the summary modal:

![alt text](/documentation/images/summary-modal-change-section-score.png)

You will be asked to provide a rationale for your decision: 

![alt text](/documentation/images/summary-modal-change-section-score-rationale.png)

## 5. Change the Assessment's Status to `Ready to Review`:

When you've finished creating/editing all the Assertions that you want, change the Assessment's status to "Ready to Review." This indicates that the Assessment is complete and ready for final sign-off.

![alt text](/documentation/images/ready-for-review.png)