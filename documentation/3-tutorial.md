# Tutorial: How To Complete An Assessment

[TODO] /17-7673779-C-G/ncit:C3359

The following is a guide outlining how to utilize VarCat to complete an Assessment of a variant/disease pairing utilizing the [ClinGen/CGC/VICC Oncogenicity SOP](https://cancervariants.org/research/standards/onc_path_sop/) and [AMP/ASCO/CAP guidelines](https://pubmed.ncbi.nlm.nih.gov/27993330/) to evaluate **oncogenicity**, **therapeutic response**, **prognostic evidence**, and **diagnostic evidence**.

## 1. Open an Assessment
From the homepage, open an Assessment by either:

  - a) Selecting an Assessment from the list, or 
  - b) Entering a variant/disease pairing of your choosing in the selection form above the table. 

![alt text](/documentation/images/landing-page.png)

## 2. Change the Assessment's Status to `Active`:

In order to edit an Assessment, you must set its [status](./1-concepts.md#assessment-status-lifecycle) to `Active` via the status button in the upper-right hand corner. Depending on the Assessment's current status, you may need to cycle through several stages before reaching `Active`:

![alt text](/documentation/images/start-assessment.png)

Only one person may edit an Assessment at a time. If your Assessment is already active, but is checked out to someone else, you will need to overtake the Assessment from them:

![alt text](/documentation/images/overtake-assessment.jpg)


## 3. Examine & Edit the Auto-Computed Oncogenicity Assertion:

VarCat automatically pulls in data from a variety of sources, and uses this evidence to auto-generate an initial Oncogenicity Assertion for the Assessment. Evaluate each section of this Assertion to **add additional evidence** that you've curated yourself, change the section's **code**, and/or update the section's **score** as applicable.

![alt text](/documentation/images/edit-onco-evidence-scode.png)
<figcaption><i>Editing a section's evidence code</i></figcaption>


## 4. [Optional] Add Additional Assertions:
In addition to the required Oncogenicity Assertion, all Assessments may optionally include one or more additional Assertions following the [AMP/ASCO/CAP](https://pubmed.ncbi.nlm.nih.gov/27993330/) guidelines.

To view an Assertion that's already been created, click on the corresponding tab in the Summary Modal:

![alt text](/documentation/images/summary-tab-diagnostic-inclusion.png)

To add or edit the Assertion's evidence, or to create a new Assertion, click on the appropriate [Evidence Tab](./2-anatomy_of_an_assessment.md#4-evidence-tabs) beneath the summary modal:

![alt text](/documentation/images/evidence-tab-diagnostic-click.png)

Here you'll see a list of evidence that's relevant to this Assessment's **variant** or its **gene.** Toggle back and forth between these views using the toggle at the top of the chart:

![alt text](/documentation/images/case-control-gene.png)

![alt text](/documentation/images/case-control-variant.png)

VarCat will pull in evidence for these tables automatically where possible. Additionally, you may also manually curate evidence by selecting the "Add Evidence" button to the upper right of the table, which will open the evidence curation form:

![alt text](/documentation/images/add-evidence-click.png)

![alt text](/documentation/images/add-evidence-modal.png)

If the evidence you'd like to use has not already been applied to the Assertion, you can apply it now by using the dropdown in the "Apply As" column:

![alt text](/documentation/images/apply-evidence.png)

Notice that the Summary Modal updates to display the newly-applied evidence, grouped by **type** (note: you may need to refresh the page). The Assertion's **score** and **classification** will also update based on the evidence you apply and how you apply it.

![alt text](/documentation/images/summary-modal-updated.png)

To manually upgrade or downgrade all evidence in a given category, use the dropdown options in the summary modal:

![alt text](/documentation/images/summary-modal-change-section-score.png)

You will be asked to provide a rationale for your decision: 

![alt text](/documentation/images/summary-modal-change-section-score-rationale.png)


## 6. Change the Assessment's Status to `Ready to Review`:

When you've finished creating/editing all the Assertions to your satisfaction, change the Assessment's status to `Ready to Review`. This indicates that the Assessment is complete and ready for final sign-off.

![alt text](/documentation/images/ready-for-review.png)