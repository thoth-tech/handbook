# Epic FSVA-54 - Link to Download super choice form

## Background / Context

Employees currently would click on a link to take them to the ATO’s website to fill in a blank
superannuation form (Standard choice form (PDF, 341KB)This link will download a file).

- Is this well used?
- Has there been surveys to show that it would be good if we can have a pre-filled form given
  employees may have provided that information before?

## Business Value

To minimise the double handling of super choice information by employers and also requiring
employees to fill in the super form, the business would like to explore the possibility of having
the forms pre-filled based on the information given by the employees to date. This will not only
make it more convenient and efficient as part of the onboarding process, but also minimise the human
error that may come with manual handling of the super info.

## In Scope

Part of Employee onboarding process Employees who were onboarded via Flare onboarding process

## Out of Scope

Employees who are not initially onboarded by the Flare onboarding process?

## What needs to happen

The current link to download a file shows only if Employee are not initially onboarded via Flare.
This link is relabelled to “Download standard choice form from ATO website”. This link is not
visible when Employee was onboarded via Flare. If Employee was onboarded via Flare, this link will
appear: “Download pre-filled standard choice form.”

- Are there minimum validation rules for form fill we need to consider?
- Does the UI need to show what parts of the super choice form hasn’t been filled?

## Assumptions / Dependencies

- Flare API can meet the performance NFR (Non-Functional Requirement)
- The super details entered by employees onboarded via Flare has been validated previously

## UX/UI Considerations

Do we provide both links or hide the one that least applies? Do we still give them the choice of
getting the blank form?

## Analytics Considerations

Capture how many employees use the pre-filled form link vs the blank form link Do we currently
capture the usage of the generic blank form link?

## Reg & Compliance Considerations

Not known

## Operations / Support / Training Considerations

Advise teams 2 weeks in advance of planned release

What are the challenges? What is a reasonable measure / response time to produce and download the
pre-filled form?

## Acceptance criteria

(Informal)

- Test with employees who were onboarded via Flare onboarding
- Test with employees who were not onboarded via Flare onboarding
- (NFR) Test pre-filled form is produced within 10 seconds
- (If applicable) test with employees onboarded via Flare who have not completed super choice
  details
- (If applicable) test with employees onboarded via Flare who have provided super choice details but
  are not valid
