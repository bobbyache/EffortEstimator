# Use Case: New WorkItem

## Screens
![New Work Item](https://uml-services.xchangedocs.co.za/svg/RP0n2y9038Nt_ehGLGkw2eAeYqi7BJY8XN0-j7XtBKsiW_hVxNMebFgMv7BVIowt4kLQXQrIJ2cUT2phE-qKBeuYQlMQT25ekHmI_KMI97tUUGQde9GT5lIck3TJLgX5F28plae0NLDD7m8oB7-eBHhOidBm6k3vR8nis9g7PIrAJnbSrQRT4_8rIs7wa46KTbxXfMX0-Hu2hitjLyi7hJ_3JIUZkQS3DpYtWquRzWRs_CV-YLRmb_3hNm00 "New Work Item")

## Description

![new-workitem-robustness](https://uml-services.xchangedocs.co.za/svg/TLB1JiCm3BtlAwpU-mCxJO83FG071fnDQus8DAaIPzN-7iT9jmM9dfxzdfrdkuV863ZDTWVouSW-GFSUANI04P809SYnuGjqdpxy34opigiHfFINJsx2888NMc4JmTiOY9ngey8_uW-qPa8sti4pnOWdKkrSy4xLsGBqjHxsyBf86sL6xpXu2vrGo0IELYqlOIinRacihABIeFRicuhIgxyRRfFrzxNRGevuYjgN1RICOLlcuOmQxW7jcAnEVgHv4LILEMYKZtGcwvTPuYUVGddhEwFMn-3EUPamP8lmps9LKkfqb3pJrVSjSxLxIsLVU_1BRedMNbhwpa_DrQTofbwpoPMZIkLswWEvINx2Nm00 "new-workitem-robustness")


### Primary Flow
The User elects to create a new WorkItem. The system presents the User with the New WorkItem Screen. The User enters a Title for the WorkItem. The user adds Tags to the WorkItem. The User inputs a Development value in Hours. The User optionally assigns a Calculation Template option. The user clicks Save. The system creates a new WorkItem and applies the Default Calculation Template if the user has not defined one.

### Alternate Flows
- The user enters an invalid Title. The system displays the appropriate validation message. The system displays the appropriate validation method and does not allow the user to continue.
- The user enters an invalid Development value or neglects to enter a value. The system displays the appropriate validation method and does not allow the User to continue.
- The user elects to cancel the process. The system closes the New Work Item Screen.


## Appendix

### References

### To Be Done

