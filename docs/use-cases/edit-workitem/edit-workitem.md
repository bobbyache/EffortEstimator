# Use Case: Edit WorkItem

## Screens

![Edit Work Item](https://uml-services.xchangedocs.co.za/svg/fLJVIyCm47xVNt4K18Us-8E120ErJfmFFco5FOmLOdjkmJGfILePS_-xYPDihEaSU2_vzTtTzzqbkLEQIAq8qn308ASQ9a9-m51Z4NGwO6nrzZDOw_Vt871wVHtru5bKKdKTB0n3Dr-vMNDbBTZ6IgXc63GGZwWoIKjD1OV6uMeyR6xkUubtA9RmQHDfcmCMA37o-qN_sbqt2NezOr6KWYFNy0N181pJEIUwagXWWcymHbdJp5CAQmcPA-jLrELvfH0oebgGiU3lD4UU8PnOZvkU7pT2PVfdK0Rp8XRSZueYVn6cCrFhK6MYn1nENuKsZ5XMCQ8nxnvHeDtBuegM1WajscJzXhUTJR0eRQPRmprz88fcRaXGQHXoZLpH6Y4rAf78RB7TIy5uJKSOEi8pRqB39dQIu8aYovMVskRYrSX4MVmsz_AY7UeeMTnLr6j7MZ6Kp_yA68iSJTIQukSFj2takatdVMwUjoaiOKVeB9bOEfa7wJyIJM30jLmUKh2sxJ0CPfks5ABsDAH9lTD-lFDrkUiw9YQipH0JypBOhCLzCrjtxf3dzdVy1W00 "Edit Work Item")

--- 

## Domain Dictionary

| Class | Description |
| --- | --- |
| Estimation Template | A template that defines default values for absolute and relative estimation metric fields. These fields are summed up to provide a final estimate of the work item. Some examples of an estimation template could be Basic, Test Intensive, Research Intensive, Spike, etc. |
| Estimation Fields | A collection of absolute and relative metric fields. These fields are summed up to provide a final estimate of the work item. |
| Absolute Estimation Field | The estimation field is not based on one or more value(s) within the estimation field set. |
| Relative Estimation Field | The value (ratio) is based on one or more estimation field(s) within the estimation field set. |
| Estimate | A series of absolute and relative metrics, eg. Development, Research, Testing, Code Review, Deployment, Data Entry. If a metric is relative it must be based on an absolute metric (eg. Testing = 0.7 of the absolute Development metric). Has a final value calculated on a metric (such as hours). |
| Additional Fields | Can be added to the field set and will be summed together with the rest of the fields to calculate an estimation.

---

## Description

### Primary Flow
The User elects to edit a work item. The system presents the User with the Screen. The system loads the default estimate template (Basic). The System calculates and displays the estimation total to the User. The User inputs the Title, Description, Component, Tags, Confidence, and a Resource. The User optionally chooses whether the work item is currently de-scoped.

The user edits some or all of the estimation fields.
> What happens if the user wants to maintain the current template ratio? Does the system needs a "Maintain ratio" checkbox?

The User clicks Save. The system saves the work item.

### Alternate Flows

- The User **selects another estimation template**. The system warns the user that the current estimate fields will be cleared and replaced with the new template fields. The system retrieves the absolute template field values and calculates the relative field values. The system displays these values to the user.
- The user **Adds another estimation field** to the estimation field set. The system recalculates the estimation and displays this result to the user.
- The user **Removes an estimation field** from the estimation field set. The system recalculates the estimation and displays the result to the user.

- The user omits or enters an invalid title. The system displays the appropriate validation message and does not allow the user to save.
- The user enters an invalid estimate value or neglects to enter a value. The system displays the appropriate validation method and does not allow the User to continue.
- The user elects to cancel the process. The system closes the New Work Item Screen.

---

## Appendix


### References

### To Be Done



