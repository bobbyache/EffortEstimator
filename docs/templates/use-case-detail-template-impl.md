# Use Case: Name

![Edit Work Item](https://uml-services.xchangedocs.co.za/svg/fLJVIyCm47xVNt4K18Us-8E120ErJfmFFco5FOmLOdjkmJGfILePS_-xYPDihEaSU2_vzTtTzzqbkLEQIAq8qn308ASQ9a9-m51Z4NGwO6nrzZDOw_Vt871wVHtru5bKKdKTB0n3Dr-vMNDbBTZ6IgXc63GGZwWoIKjD1OV6uMeyR6xkUubtA9RmQHDfcmCMA37o-qN_sbqt2NezOr6KWYFNy0N181pJEIUwagXWWcymHbdJp5CAQmcPA-jLrELvfH0oebgGiU3lD4UU8PnOZvkU7pT2PVfdK0Rp8XRSZueYVn6cCrFhK6MYn1nENuKsZ5XMCQ8nxnvHeDtBuegM1WajscJzXhUTJR0eRQPRmprz88fcRaXGQHXoZLpH6Y4rAf78RB7TIy5uJKSOEi8pRqB39dQIu8aYovMVskRYrSX4MVmsz_AY7UeeMTnLr6j7MZ6Kp_yA68iSJTIQukSFj2takatdVMwUjoaiOKVeB9bOEfa7wJyIJM30jLmUKh2sxJ0CPfks5ABsDAH9lTD-lFDrkUiw9YQipH0JypBOhCLzCrjtxf3dzdVy1W00 "Edit Work Item")

---
## Primary Flow

The Trusted Host requests the system to Delete a Package. The system confirms the UserGroup has eSigning turned on. The system confirms the {user} is registered at SH. The system confirms the {user} is the Package Owner.

The System requests the SigningHub to Delete the Package. SigningHub sends a 200 Success Response. The system calls Log Package Information

## Alternate Flows

- The system fails to confirm the UserGroup eSigning Status. The system returns a 500 Error Response.
- The system determines that the UserGroup has turned off eSigning and returns an Error Response.
- The system determines that the {user} isn't registered and returns an Error Response.
- The system determines that the {user} is not the Signature Request Owner and returns an Error Response.

---
## References
- Reference 1
- Reference 2
---
## To Be Actioned
- Action 1
- Action 2



