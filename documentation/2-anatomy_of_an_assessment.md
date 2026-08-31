# Anatomy of an Assessment

This page shows the main parts of an assessment view.

![](/documentation/images/assessment-anatomy.png)

## 1. Assessment Header

![Assessment header](/documentation/images/header.png)

Shows the variant and disease pairing for the current assessment.

## 2. Status Section

![Status section](/documentation/images/status-section.png)

Shows the assessment's current status and who, if anyone, has it checked out.

Use this section to:

- **Move** the assessment to the next or previous status
- **Overtake** an active assessment from another user
- **Review** the assessment's status history, including _who_ previously checked out the assessment and _when_

## 3. Summary Modal

![Summary modal](/documentation/images/summary-modal.png)

Lists all assertions in the assessment (left) and summarizes the currently-selected one (right).

For the selected assertion, the modal shows:

- **Classification**: The current conclusion drawn by this assertion
- **Score**: The current strength of support the applied evidence has for this conclusion
- **Applied Evidence**: A summary list of the evidence currently contributing to that result

Oncogenicity evidence is grouped by **strength**. Other assertions group evidence by **type**.

## 4. Evidence Tabs

These tabs contain the evidence used for each assertion.

### Oncogenicity Tab

![Oncogenicity tab](/documentation/images/evidence-section.png)

Evidence is organized into sections by evidence type. Each section has:

- Any **evidence items** of the titular type
- A **code** indicating the significance of the findings
- A **score** indicating the strength of the findings

Users can review the auto selected values, adjust them if needed, and add evidence to a section.

The overall oncogenicity assertion score is the **sum** of all individual section scores.

### Therapeutic, Diagnostic, and Prognostic Tabs

![Diagnostic evidence tab](/documentation/images/evidence-tab-diagnostic.png)

These tabs show evidence in tables. Each table may include:

- Evidence tied to the specific variant
- Evidence tied to the broader gene

Users can:

- **Apply** evidence with the `Apply As` column
- **Add** new evidence with the `Add Evidence` button
- **Edit** evidence (where editing is allowed)

The overall score for these assertion types comes from the **highest ranked** applied evidence.

### Previous Classifications Tab

![Previous classifications tab](/documentation/images/prev-classifications.png)

This tab is reference only. It shows how related variants or genes were classified in other assessments.

## 5. Table of Contents Sidebar

![Table of contents sidebar](/documentation/images/table-of-contents-sidebar.png)

Lets users jump to a section of the assessment page.
