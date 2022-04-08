# Use Case: Name

## To Be Actioned
---
- [ ] Action 1
- [ ] Action 2

## Screen(s)
---
![New Work Item](https://uml-services.xchangedocs.co.za/svg/RP0n2y9038Nt_ehGLGkw2eAeYqi7BJY8XN0-j7XtBKsiW_hVxNMebFgMv7BVIowt4kLQXQrIJ2cUT2phE-qKBeuYQlMQT25ekHmI_KMI97tUUGQde9GT5lIck3TJLgX5F28plae0NLDD7m8oB7-eBHhOidBm6k3vR8nis9g7PIrAJnbSrQRT4_8rIs7wa46KTbxXfMX0-Hu2hitjLyi7hJ_3JIUZkQS3DpYtWquRzWRs_CV-YLRmb_3hNm00 "New Work Item")

## Domain Dictionary
---

| Class | Description |
| --- | --- |
| Class | desc |

## Primary Flow
---
The Trusted Host requests the system to Delete a Package. The system confirms the UserGroup has eSigning turned on. The system confirms the {user} is registered at SH. The system confirms the {user} is the Package Owner.

The System requests the SigningHub to Delete the Package. SigningHub sends a 200 Success Response. The system calls Log Package Information

![new-workitem-robustness](https://uml-services.xchangedocs.co.za/svg/TLB1JiCm3BtlAwpU-mCxJO83FG071fnDQus8DAaIPzN-7iT9jmM9dfxzdfrdkuV863ZDTWVouSW-GFSUANI04P809SYnuGjqdpxy34opigiHfFINJsx2888NMc4JmTiOY9ngey8_uW-qPa8sti4pnOWdKkrSy4xLsGBqjHxsyBf86sL6xpXu2vrGo0IELYqlOIinRacihABIeFRicuhIgxyRRfFrzxNRGevuYjgN1RICOLlcuOmQxW7jcAnEVgHv4LILEMYKZtGcwvTPuYUVGddhEwFMn-3EUPamP8lmps9LKkfqb3pJrVSjSxLxIsLVU_1BRedMNbhwpa_DrQTofbwpoPMZIkLswWEvINx2Nm00 "new-workitem-robustness")

## Alternate Flows
---

- The system fails to confirm the UserGroup eSigning Status. The system returns a 500 Error Response.
- The system determines that the UserGroup has turned off eSigning and returns an Error Response.
- The system determines that the {user} isn't registered and returns an Error Response.
- The system determines that the {user} is not the Signature Request Owner and returns an Error Response.

## Change History
---

| Date | Stakeholder | Change |
| :--- | :--- | --- |
| 2022-01-01 | stakeholder | change |

## Appendix
---

### References
- Reference 1
- Reference 2




