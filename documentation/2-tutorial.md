# Tutorial: How to Complete an Assessment

This guide walks through a typical assessment workflow in VarCat.

## 1. Open an Assessment
From the home page, open an assessment by:

- a) Entering a variant + disease pairing in the form shown below, or
- b) Selecting a previously-created assessment from the table

![Landing page](/documentation/images/landing-page.png)

## 2. Explore the Assessment's Structure

![Assessment layout](/documentation/images/assessment-anatomy.png)

1. The **header** identifies the variant/disease pairing.
2. The **status section** shows the assessment's current [status](./1-concepts.md#assessment-statuses), checkout information, and status history. Use this section to:
    - _Move_ the assessment to the next or previous status
    - _Overtake_ an active assessment from another user
    - _Review_ the assessment's status history, including _who_ previously checked out the assessment and _when_
3. The **summary modal** lists the assessment's assertions (left) and displays a summary of the selected assertion (right), including its:
    - _Classification_: The current conclusion drawn by this assertion
    - _Score_: The current strength of support the applied evidence has for this conclusion
    - _Applied Evidence_: A summary list of the evidence currently contributing to that result
4. **Evidence tabs** contain the evidence for each assertion type.
5. The **table of contents sidebar** allows quick navigation to the various sections of the assessment.

## 3. Change the Status to `Active`
An assessment must be `Active` before you can edit it.

Use the status control in the upper right corner to move the assessment to `Active`.

![Start assessment](/documentation/images/start-assessment.png)

Only one user can edit an assessment at a time. If it is currently checked out by another user, you will need to overtake it:

![Overtake assessment](/documentation/images/overtake-assessment.jpg)


## 4. Review the Oncogenicity Assertion
VarCat creates an initial oncogenicity assertion automatically.

Oncogenicity evidence is organized into sections by type. Each section has:

- Any **evidence items** of the titular type
- A **code** indicating the significance of the findings
- A **score** indicating the strength of the findings

![Edit oncogenicity section](/documentation/images/edit-onco-evidence-scode.png)

Review each evidence section and update it as needed. You can:

- Curate your own additional evidence manually
- Revise the section's auto-selected code
- Change the section's auto-computed score

The oncogenicity assertion's overall score is the **sum** of all individual section scores.

## 5. [Optional] Add or Review Other Assertions
If needed, add or review therapeutic, diagnostic, and/or prognostic assertions.

Use the Summary Modal to view assertions that already exist:

![Summary modal diagnostic tab](/documentation/images/summary-tab-diagnostic-inclusion.png)

Click the corresponding evidence tab below to work on an existing assertion. If no assertion exists yet for that type, applying the first piece of evidence will create it automatically.

![Diagnostic evidence tab click](/documentation/images/evidence-tab-diagnostic-click.png)

Toggle between variant-level and gene-level evidence where available:

![Gene evidence view](/documentation/images/case-control-gene.png)

![Variant evidence view](/documentation/images/case-control-variant.png)

If needed, add new evidence with **Add Evidence**.

![Add evidence button](/documentation/images/add-evidence-click.png)

Apply evidence with the `Apply As` dropdown, if needed.

![Apply evidence](/documentation/images/apply-evidence.png)

After evidence is applied, the summary modal updates to reflect the assertion's current state. The assertion's overall classification and score are determined by the **highest ranked** evidence that is currently applied.

You can manually adjust the applied strength for a evidence line grouping from the summary modal. You will be asked to provide a rationale for your decision.

![Change grouped score](/documentation/images/summary-modal-change-section-score.png)


## 6. Change the Status to `Awaiting Review`
When the assessment is complete, update its status to `Awaiting Review` so it can be reviewed and signed off.

![Awaiting review](/documentation/images/ready-for-review.png)
