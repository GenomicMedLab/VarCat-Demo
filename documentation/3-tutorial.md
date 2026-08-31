# Tutorial: How to Complete an Assessment

This guide walks through a typical assessment workflow in VarCat.

## 1. Open an Assessment
From the home page, open an assessment by:

- a) Entering a variant + disease pairing in the form (shown below), or
- b) Selecting a previously-created assessment from the table

![Landing page](/documentation/images/landing-page.png)

## 2. Change the Status to `Active`
An assessment must be `Active` before you can edit it.

Use the status control in the upper right corner to move the assessment to `Active`.

![Start assessment](/documentation/images/start-assessment.png)

Only one user can edit an assessment at a time. If another user has it checked out, you will need to overtake it before continuing.

![Overtake assessment](/documentation/images/overtake-assessment.jpg)

## 3. Review the Oncogenicity Assertion
VarCat creates an initial oncogenicity assertion automatically.

Review each evidence section and update it as needed. You can:

- Curate your own additional evidence manually
- Revise the section's auto-selected code
- Change the section's auto-computed score

![Edit oncogenicity section](/documentation/images/edit-onco-evidence-scode.png)

## 4. [Optional] Add or Review Other Assertions
If needed, add or review therapeutic, diagnostic, and/or prognostic assertions.

Use the Summary Modal to view assertions that already exist:

![Summary modal diagnostic tab](/documentation/images/summary-tab-diagnostic-inclusion.png)

To create a new assertion or work on an existing one, click on the corresponding evidence tab below the summary:

![Diagnostic evidence tab click](/documentation/images/evidence-tab-diagnostic-click.png)

Toggle between variant-level and gene-level evidence where available:

![Gene evidence view](/documentation/images/case-control-gene.png)

![Variant evidence view](/documentation/images/case-control-variant.png)

If needed, add new evidence with **Add Evidence**.

![Add evidence button](/documentation/images/add-evidence-click.png)

Apply evidence with the `Apply As` dropdown, if needed.

![Apply evidence](/documentation/images/apply-evidence.png)

After evidence is applied, the Summary Modal updates to reflect the current classification, score, and applied evidence.

![Updated summary modal](/documentation/images/summary-modal-updated.png)

You can also adjust the applied strength for a grouped category from the Summary Modal.

![Change grouped score](/documentation/images/summary-modal-change-section-score.png)

You will be asked to provide a rationale for your decision: 

![Grouped score rationale](/documentation/images/summary-modal-change-section-score-rationale.png)

## 6. Change the Status to `Awaiting Review`
When the assessment is complete, move it to `Awaiting Review` so it can be reviewed and signed off.

![Awaiting review](/documentation/images/ready-for-review.png)
