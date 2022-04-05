# Use Case: Edit WorkItem

## Screens

![Edit Work Item](https://uml-services.xchangedocs.co.za/svg/fLJVIyCm47xVNt4K18Us-8E120ErJfmFFco5FOmLOdjkmJGfILePS_-xYPDihEaSU2_vzTtTzzqbkLEQIAq8qn308ASQ9a9-m51Z4NGwO6nrzZDOw_Vt871wVHtru5bKKdKTB0n3Dr-vMNDbBTZ6IgXc63GGZwWoIKjD1OV6uMeyR6xkUubtA9RmQHDfcmCMA37o-qN_sbqt2NezOr6KWYFNy0N181pJEIUwagXWWcymHbdJp5CAQmcPA-jLrELvfH0oebgGiU3lD4UU8PnOZvkU7pT2PVfdK0Rp8XRSZueYVn6cCrFhK6MYn1nENuKsZ5XMCQ8nxnvHeDtBuegM1WajscJzXhUTJR0eRQPRmprz88fcRaXGQHXoZLpH6Y4rAf78RB7TIy5uJKSOEi8pRqB39dQIu8aYovMVskRYrSX4MVmsz_AY7UeeMTnLr6j7MZ6Kp_yA68iSJTIQukSFj2takatdVMwUjoaiOKVeB9bOEfa7wJyIJM30jLmUKh2sxJ0CPfks5ABsDAH9lTD-lFDrkUiw9YQipH0JypBOhCLzCrjtxf3dzdVy1W00 "Edit Work Item")

## Description

### Primary Flow
The User elects to edit a WorkItem. The system presents the User with the Edit WorkItem Screen. The system loads the DefaultCalculationTemplate and adds the templates RelativeTimeEstimate to the WorkItem TimeEstimate Total. The System displays this Total to the User. The User inputs the Title, Description, Component, Tags, Confidence, and a Resource. The User optionally chooses whether the WorkItem is currently de-scoped.

The User clicks Save. The system saves the WorkItem together with its additional fields, resource, and calculation estimate values.

The User selects a CalculationTemplate. The system adds the template RelativeTimeEstimates to the WorkItem based on a relative calculation (based on the DefaultTimeEstimate). The system calculates and presents the expected duration to the User. The user selects a TimeEstimate. The User inputs a more appropriate value. The system calculates and presents the expected duration to the user.



### Alternate Flows

- **Use Case** The user removes a TimeEstimate from the WorkItem.
- **Use Case** The user adds a TimeEstimate to the WorkItem.
- **Use Case** The modifies a TimeEstimate to a more appropriate value
- The user enters an invalid Title. The system displays the appropriate validation message. The system displays the appropriate validation method and does not allow the user to continue.
- The user enters an invalid estimate value or neglects to enter a value. The system displays the appropriate validation method and does not allow the User to continue.
- The user elects to cancel the process. The system closes the New Work Item Screen.

## Appendix

### References

### To Be Done



