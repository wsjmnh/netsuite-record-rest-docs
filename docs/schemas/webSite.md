# Schemas: webSite

Property tables for definitions owned by `webSite`.

Record page: [webSite](../records/webSite.md).

## Index

- [webSite](#website) — 208 properties
- [webSite-entryPointsCollection](#website-entrypointscollection) — 6 properties
- [webSite-entryPointsElement](#website-entrypointselement) — 10 properties
- [webSite-fieldsetCollection](#website-fieldsetcollection) — 6 properties
- [webSite-fieldsetElement](#website-fieldsetelement) — 7 properties
- [webSiteCollection](#websitecollection) — 6 properties
- [webSiteSelectOptions](#websiteselectoptions) — 48 properties

## webSite

Browser definition `webSite`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `analyticsClickAttributes` | Analytics Click Attributes | string |  |  |  |  |
| `analyticsSubmitAttributes` | Analytics Submit Attributes | string |  |  |  |  |
| `assignNewCustomersToSite` | Assign New Customers to this Site | boolean |  |  |  |  |
| `autoDownloadMedia` | Automatically download published site media items | boolean |  |  |  |  |
| `bSendCheckoutErrorEmail` | Send email of Checkout errors | boolean |  |  |  |  |
| `bSendDownloadAvailableEmail` | Send email that Download is available | boolean |  |  |  |  |
| `bSendGiftCertificateConfEmail` | Send Gift Certificate Confirmation email | boolean |  |  |  |  |
| `bSendGiftCertificateEmail` | Send Gift Certificate email | boolean |  |  |  |  |
| `bSendLicenseCodeEmail` | Send License Code email | boolean |  |  |  |  |
| `bSendOrderApprovedConfEmail` | Send email when order is approved | boolean |  |  |  |  |
| `bSendOrderCancelledConfEmail` | Send email when order is cancelled | boolean |  |  |  |  |
| `bSendOrderFulfilledConfEmail` | Send email when order is fulfilled | boolean |  |  |  |  |
| `bSendOrderReceivedConfEmail` | Send email when order is received | boolean |  |  |  |  |
| `bSendPasswordRecoveryEmail` | Send Password Recovery email | boolean |  |  |  |  |
| `bSendRegistrationConfEmail` | Send Registration Confirmation Email | boolean |  |  |  |  |
| `bStrApproveOrderCopy` | Send BCC Order Approved Emails | boolean |  |  |  |  |
| `bStrCancelOrderCopy` | Send BCC Order Cancelled Emails | boolean |  |  |  |  |
| `bStrEmailCopy` | Send BCC Order Received Emails | boolean |  |  |  |  |
| `bStrEmailGiftConfCopy` | Send BCC Gift Certificate Confirmation Emails | boolean |  |  |  |  |
| `bStrEmailGiftCopy` | Send BCC Gift Certificate Emails | boolean |  |  |  |  |
| `bStrFulfillOrderCopy` | Send BCC Order Fulfilled Emails | boolean |  |  |  |  |
| `bStrRegistrationConfCopy` | Send BCC Registration Confirmation Emails | boolean |  |  |  |  |
| `cartDisplayOrder` |  | object |  |  |  |  |
| `cartDisplayOrder.id` | Internal identifier | string |  |  |  | `RECENT_LAST`, `RECENT_FIRST` |
| `cartDisplayOrder.refName` | Reference Name | string |  |  |  |  |
| `cartUpsellItems` |  | object |  |  |  |  |
| `cartUpsellItems.id` | Internal identifier | string |  |  |  | `UPSELL_FIRST_RELATED_NEXT`, `ONLY_UPSELL_ITEMS`, `RELATED_FIRST_UPSELL_NEXT`, `ONLY_RELATED_ITEMS` |
| `cartUpsellItems.refName` | Reference Name | string |  |  |  |  |
| `categoryListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `ccFormTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `ccRequireAuth` | Process an online payment with Sales Order creation | boolean |  |  |  |  |
| `checkoutErrorEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `chromaSubsampling` | Chroma Subsampling | boolean |  |  |  |  |
| `colorSet` |  | object |  |  |  |  |
| `colorSet.id` | Internal identifier | string |  |  |  | `88`, `89`, `-380`, `-10`, `-11`, `-12`, `-13`, `-651`, `-376`, `-134`, `-14`, `-650`, `-375`, `-133`, `-15`, `-653`, `-378`, `-136`, `-16`, `-652`, `-377`, `-135`, `-372`, `-130`, `-371`, `-374`, `-132`, `-373`, `-131`, `90`, `91`, `93`, `94`, `-138`, `95`, `-379`, `-137`, `96`, `97`, `-139`, `98`, `99`, `-150`, `-145`, `0`, `-144`, `-147`, `-146`, `-141`, `-140`, `-143`, `-142`, `-149`, `-148`, `-161`, `-160`, `-156`, `-155`, `-158`, `-157`, `-152`, `-151`, `-154`, `-153`, `-159`, `-2`, `-5`, `-6`, `-7`, `-8`, `-9`, `-101`, `-100`, `-103`, `-102`, `-109`, `-108`, `-105`, `-104`, `-107`, `-106`, `67`, `68`, `69`, `-354`, `-112`, `-353`, `-111`, `-356`, `-114`, `-355`, `-113`, `-350`, `-352`, `-110`, `-351`, `-119`, `70`, `71`, `72`, `-358`, `-116`, `73`, `-357`, `-115`, `74`, `-118`, `75`, `-359`, `-117`, `76`, `77`, `78`, `79`, `-370`, `-365`, `-123`, `-364`, `-122`, `-367`, `-125`, `-366`, `-124`, `-361`, `-481`, `-360`, `-363`, `-121`, `-362`, `-120`, `80`, `81`, `82`, `83`, `-369`, `-127`, `84`, `-368`, `-126`, `85`, `-129`, `86`, `-128`, `87` |
| `colorSet.refName` | Reference Name | string |  |  |  |  |
| `compressedImageQuality` | Compressed Image Quality | string |  |  |  |  |
| `confPageTrackingHtml` | Order Tracking Script HTML | string |  |  |  |  |
| `cookiePolicy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createCustomersAsCompanies` | Create Customers as Companies | boolean |  |  |  |  |
| `custromeRegistrationType` |  | object |  |  |  |  |
| `custromeRegistrationType.id` | Internal identifier | string |  |  |  | `OPTANON`, `MANDATORY`, `DISALLOWED`, `ALLANON` |
| `custromeRegistrationType.refName` | Reference Name | string |  |  |  |  |
| `defaultCustomerCategory` |  | customerCategory |  |  | [`customerCategory`](customerCategory.md#customercategory) |  |
| `defaultHostingRoot` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultShippingMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `descriptionFontSize` | Description Font Size | integer | int64 |  |  |  |
| `dispFirstLastnameSeparately` | Display First and Last Name in Separate Fields on Registration Page | boolean |  |  |  |  |
| `displayCompanyField` | Display Company Field on Registration Page | boolean |  |  |  |  |
| `displayName` | Display Name | string |  |  |  |  |
| `displayUnsubscribe` | Display Unsubscribe to Email Checkbox on Registration Page | boolean |  |  |  |  |
| `doctypeHtml` | Document Type | string |  |  |  |  |
| `downloadAvailableEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `emailFooter` | Footer Text | string |  |  |  |  |
| `emailHeader` | Header Text | string |  |  |  |  |
| `enableGAIntegration` | Enable Google Analytics Integration | boolean |  |  |  |  |
| `entryPoints` |  | webSite-entryPointsCollection |  |  | [`webSite-entryPointsCollection`](#website-entrypointscollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `fieldset` |  | webSite-fieldsetCollection |  |  | [`webSite-fieldsetCollection`](#website-fieldsetcollection) |  |
| `font` |  | object |  |  |  |  |
| `font.id` | Internal identifier | string |  |  |  | `OCRB`, `Garamond`, `Trebuchet`, `Times-Roman`, `Univers`, `OCRA`, `MS Gothic`, `Myriad Pro`, `BARCODE`, `Helvetica`, `Times New Roman`, `Arial`, `Gothic`, `NotoSansArabic`, `Palatino`, `Verdana`, `Tahoma`, `ComicSans`, `UniversCondensed`, `Georgia`, `Open Sans` |
| `font.refName` | Reference Name | string |  |  |  |  |
| `giftCerteAffectsMinAmount` | Gift Certificate Affects Minimum Order Amount | boolean |  |  |  |  |
| `giftCertificateConfEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `giftCertificateEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `hidePaymentPageWhenNoBalance` | Hide Payment Page If Order Total Equals Zero | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `igniteEdition` |  | object |  |  |  |  |
| `igniteEdition.id` | Internal identifier | string |  |  |  | `STANDARD`, `ADVANCED` |
| `igniteEdition.refName` | Reference Name | string |  |  |  |  |
| `includeUncategorizedItems` | Show Uncategorized Items | boolean |  |  |  |  |
| `includeVatWithPrices` | Prices Include Tax | boolean |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `internalName` | Internal Name | string |  |  |  |  |
| `invoiceFormTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPrimary` | Primary | string |  |  |  |  |
| `isScriptableCartAndCheckout` | Scriptable Cart and Checkout | boolean |  |  |  |  |
| `isWebstoreOffline` | Take Website Offline for Maintenance | boolean |  |  |  |  |
| `isWsdk` | WSDK | boolean |  |  |  |  |
| `itemListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemTemplateAccountingtItem` |  | object |  |  |  |  |
| `itemTemplateAccountingtItem.id` | Internal identifier | string |  |  |  | `-134`, `-178`, `-133`, `-177`, `-136`, `-179`, `-135`, `-130`, `-174`, `-173`, `-176`, `-132`, `-131`, `-175`, `-138`, `-137`, `-139`, `-150`, `-101`, `-145`, `-144`, `-100`, `-103`, `-147`, `-102`, `-146`, `-141`, `-140`, `-143`, `-142`, `-109`, `-108`, `-149`, `-105`, `-148`, `-104`, `-107`, `-106`, `-161`, `-160`, `-156`, `-112`, `-111`, `-155`, `-158`, `-114`, `-157`, `-113`, `-110`, `-154`, `-153`, `-119`, `-116`, `-159`, `-115`, `-118`, `-117`, `-170`, `-172`, `-171`, `-123`, `-122`, `-125`, `-124`, `-162`, `-121`, `-120`, `-127`, `-126`, `-129`, `-128` |
| `itemTemplateAccountingtItem.refName` | Reference Name | string |  |  |  |  |
| `itemTemplateInformationItem` |  | object |  |  |  |  |
| `itemTemplateInformationItem.id` | Internal identifier | string |  |  |  | `-134`, `-178`, `-133`, `-177`, `-136`, `-179`, `-135`, `-130`, `-174`, `-173`, `-176`, `-132`, `-131`, `-175`, `-138`, `-137`, `-139`, `-150`, `-101`, `-145`, `-144`, `-100`, `-103`, `-147`, `-102`, `-146`, `-141`, `-140`, `-143`, `-142`, `-109`, `-108`, `-149`, `-105`, `-148`, `-104`, `-107`, `-106`, `-161`, `-160`, `-156`, `-112`, `-111`, `-155`, `-158`, `-114`, `-157`, `-113`, `-110`, `-154`, `-153`, `-119`, `-116`, `-159`, `-115`, `-118`, `-117`, `-170`, `-172`, `-171`, `-123`, `-122`, `-125`, `-124`, `-162`, `-121`, `-120`, `-127`, `-126`, `-129`, `-128` |
| `itemTemplateInformationItem.refName` | Reference Name | string |  |  |  |  |
| `legacyCategoryDescriptions` | Legacy Category Descriptions | boolean |  |  |  |  |
| `legacyDenseListSupport` | Legacy Dense List Layout | boolean |  |  |  |  |
| `legacyImageAttributeTags` | Legacy Tag Support for Images | boolean |  |  |  |  |
| `legacyNavigationLinks` | Legacy Navigation Style | boolean |  |  |  |  |
| `legacyWelcomePage` | Legacy Welcome Page Style | boolean |  |  |  |  |
| `licenseCodeEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `loginAllowed` | Allow Login / Register | boolean |  |  |  |  |
| `minimumOrderAmount` | Minimum Order Amount | number | double |  |  |  |
| `noActivateTabOnHostedPages` | Don't Activate Hosted Page Tabs | boolean |  |  |  |  |
| `nonCcPayMethodsAllowed` | Allow non-credit card payment methods during Checkout | boolean |  |  |  |  |
| `onlinePriceLevel` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `orderApprovedConfEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderCancelledConfEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderFulfilledConfEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderReceivedConfEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `outputLineBreaksAsBr` | Output Line Breaks as &lt;br&gt; | boolean |  |  |  |  |
| `pageWidth` | Page Width | string |  |  |  |  |
| `passPromoCodeToCheckout` | Pass URL Promotion Code to Checkout | boolean |  |  |  |  |
| `passwordRecoveryEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentProcessingProfiles` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `registrationConfEmail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `relatedItemsDescription` | Related Items Description | string |  |  |  |  |
| `relatedItemsLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `requestShippingAddressFirst` | Ask For Shipping Address First | boolean |  |  |  |  |
| `requireCompanyField` | Mandatory Company Field on Registration Page | boolean |  |  |  |  |
| `requireLoginForPricing` | Require Login For Pricing | boolean |  |  |  |  |
| `requireShippingInformation` | Shipping Information is Required | boolean |  |  |  |  |
| `requireTermsAndConditions` | Require Terms and Conditions | boolean |  |  |  |  |
| `sApproveOrderCopyEmail` | BCC Order Approved Recipient Emails | string |  |  |  |  |
| `sCancelOrderCopyEmail` | BCC Order Canceled Recipient Emails | string |  |  |  |  |
| `sEmailAddrForError` | Send email of Checkout errors to address | string |  |  |  |  |
| `sFromCheckoutErrorEmail` | Send email of Checkout errors from address | string |  |  |  |  |
| `sFromDownloadAvailableEmail` | Download availability email sent from address | string |  |  |  |  |
| `sFromGiftCertificateConfEmail` | Gift Certificate Confirmation sent from email address | string |  |  |  |  |
| `sFromGiftCertificateEmail` | Gift Certificate sent from email address | string |  |  |  |  |
| `sFromLicenseCodeEmail` | Send License Code email from this address | string |  |  |  |  |
| `sFromOrderApprovedConfEmail` | Order approval email sent from address | string |  |  |  |  |
| `sFromOrderCancelledConfEmail` | Canceled order email sent from address | string |  |  |  |  |
| `sFromOrderFulfilledConfEmail` | Order fulfillment email sent from address | string |  |  |  |  |
| `sFromOrderReceivedConfEmail` | Order received email sent from address | string |  |  |  |  |
| `sFromPasswordRecoveryEmail` | Send Password Recovery email from this address | string |  |  |  |  |
| `sFromRegistrationConfEmail` | Registration Confirmation email sent from address | string |  |  |  |  |
| `sFulfillOrderCopyEmail` | BCC Order Fulfilled Recipient Emails | string |  |  |  |  |
| `sRegistrationConfEmailCopy` | BCC Registration Confirmation Recipient Emails | string |  |  |  |  |
| `sStoreEmailAddrForCopy` | BCC Order Received Recipient Emails | string |  |  |  |  |
| `sStoreEmailAddrForGiftConfCopy` | BCC Gift Certificate Confirmation Recipient Emails | string |  |  |  |  |
| `sStoreEmailAddrForGiftCopy` | BCC Gift Certificate Recipient Emails | string |  |  |  |  |
| `salesOrderType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `saveCreditInfo` | Save Credit Card Info by Default | boolean |  |  |  |  |
| `scriptTemplateCreditCard` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `scriptTemplateInvoice` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `searchCategoryListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `searchForCategories` | Include Categories in Search Results | boolean |  |  |  |  |
| `searchForInformationItems` | Include Information Items in Search Results | boolean |  |  |  |  |
| `searchFormItemListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `searchItemListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `searchLinkForm` |  | object |  |  |  |  |
| `searchLinkForm.id` | Internal identifier | string |  |  |  |  |
| `searchLinkForm.refName` | Reference Name | string |  |  |  |  |
| `searchPortletForm` |  | object |  |  |  |  |
| `searchPortletForm.id` | Internal identifier | string |  |  |  |  |
| `searchPortletForm.refName` | Reference Name | string |  |  |  |  |
| `shipsToAllCountries` | Website Ships to All Countries | boolean |  |  |  |  |
| `showBillingAddress` | Display Billing Address | boolean |  |  |  |  |
| `showCartSummaryPortlet` | Show Cart Summary | boolean |  |  |  |  |
| `showCookieConsentBanner` | Show Cookie Consent Banner | boolean |  |  |  |  |
| `showCurrencyPortlet` | Show Website Currency | boolean |  |  |  |  |
| `showExtendedCart` | Show Extended Cart | boolean |  |  |  |  |
| `showNavigationPortlet` | Show Navigation Portlet | boolean |  |  |  |  |
| `showOrderTrackinglink` | Display Order Tracking Link | boolean |  |  |  |  |
| `showPOFieldOnPayment` | Display Purchase Order Field on Payment Info Page | boolean |  |  |  |  |
| `showQuantityPricinginLists` | Show Quantity Pricing in Lists | boolean |  |  |  |  |
| `showSaveCreditInfo` | Display 'Save My Credit Card Info' Field | boolean |  |  |  |  |
| `showSearchPortlet` | Show Search | boolean |  |  |  |  |
| `showShippingEstimator` | Show Shipping Estimator in Cart | boolean |  |  |  |  |
| `showTellAFriendLink` | Show "Tell a Friend" Link | boolean |  |  |  |  |
| `siteLoginRequired` | Password-Protect Entire Site | boolean |  |  |  |  |
| `sitePortletStyle` |  | object |  |  |  |  |
| `sitePortletStyle.id` | Internal identifier | string |  |  |  | `HEADERBAR`, `HEADERBARSM`, `JOINED`, `ROUNDEDCAPS`, `TRANSPARENT`, `BOXED` |
| `sitePortletStyle.refName` | Reference Name | string |  |  |  |  |
| `siteTabAlignment` |  | object |  |  |  |  |
| `siteTabAlignment.id` | Internal identifier | string |  |  |  | `CENTER`, `LEFT`, `RIGHT` |
| `siteTabAlignment.refName` | Reference Name | string |  |  |  |  |
| `siteTabStyle` |  | object |  |  |  |  |
| `siteTabStyle.id` | Internal identifier | string |  |  |  | `STANDARDTABS`, `TABBAR`, `LINKS`, `BUTTONBAR`, `RECTTABS`, `CURVEDTABS`, `DEFAULT` |
| `siteTabStyle.refName` | Reference Name | string |  |  |  |  |
| `siteUsesCartTags` | Site Uses Cart Summary Tags | boolean |  |  |  |  |
| `siteUsesDropShadows` | Site Uses Drop Shadows | boolean |  |  |  |  |
| `storeEmail` | Default Website Email From Address | string |  |  |  |  |
| `stripMetadata` | Strip metadata | boolean |  |  |  |  |
| `termsAndConditionsHtml` | Terms and Conditions HTML | string |  |  |  |  |
| `titleFontSize` | Title Font Size | integer | int64 |  |  |  |
| `upsellDescription` | Upsell Description | string |  |  |  |  |
| `upsellItems` |  | object |  |  |  |  |
| `upsellItems.id` | Internal identifier | string |  |  |  | `UPSELL_FIRST_RELATED_NEXT`, `ONLY_UPSELL_ITEMS`, `RELATED_FIRST_UPSELL_NEXT`, `ONLY_RELATED_ITEMS` |
| `upsellItems.refName` | Reference Name | string |  |  |  |  |
| `upsellItemsLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `upsellMinimumCorrelation` | Minimum Correlation % for Upsell | number | double |  |  |  |
| `upsellMinimumCount` | Minimum Number of Buyers for Upsell | integer | int64 |  |  |  |
| `upsellMinimumLift` | Minimum Lift % for Upsell | number | double |  |  |  |
| `useUrlFileExtension` | Use File Extension | boolean |  |  |  |  |
| `websiteLogo` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `websiteLogoAlign` |  | object |  |  |  |  |
| `websiteLogoAlign.id` | Internal identifier | string |  |  |  | `CENTER`, `LEFT`, `RIGHT` |
| `websiteLogoAlign.refName` | Reference Name | string |  |  |  |  |
| `websiteLogoLinkUrl` | Logo Link URL | string |  |  |  |  |
| `websiteScope` |  | object |  |  |  |  |
| `websiteScope.id` | Internal identifier | string |  |  |  | `SUITE_COMMERCE_IN_STORE`, `SUITE_COMMERCE`, `FULL_WEB_STORE`, `INFO_CATALOG_PRICING`, `INFO_CATALOG`, `SUITE_COMMERCE_MY_ACCOUNT`, `INFO_ONLY`, `SUITE_COMMERCE_ADVANCED` |
| `websiteScope.refName` | Reference Name | string |  |  |  |  |
| `websiteTheme` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `webstoreAddItemBehavior` |  | object |  |  |  |  |
| `webstoreAddItemBehavior.id` | Internal identifier | string |  |  |  | `SHOWCART`, `SAMEPAGE` |
| `webstoreAddItemBehavior.refName` | Reference Name | string |  |  |  |  |
| `webstoreMetaTags` | Addition to <head> | string |  |  |  |  |
| `wsdkCancelCartUrl` | Shopping cart page Continue Shopping link URL | string |  |  |  |  |
| `wsdkCancelCheckoutUrl` | Checkout page Cancel link URL | string |  |  |  |  |
| `wsdkCancelLoginUrl` | Login/registration page Cancel link URL | string |  |  |  |  |
| `wsdkCompleteCheckoutUrl` | URL to go to after checkout is complete | string |  |  |  |  |
| `wsdkCompleteLoginUrl` | URL to go to after login/registration is complete | string |  |  |  |  |

## webSite-entryPointsCollection

Browser definition `webSite-entryPointsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | webSite-entryPointsElement[] |  |  | [`webSite-entryPointsElement`](#website-entrypointselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## webSite-entryPointsElement

Browser definition `webSite-entryPointsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `entrypath` | Path | string |  |  |  |  |
| `entrytype` |  | object |  |  |  |  |
| `entrytype.id` | Internal identifier | string |  |  |  | `LOGOUT`, `REGISTER`, `CHECKOUT`, `HOMEPAGE`, `LOGIN`, `CUSTCENTER`, `CART` |
| `entrytype.refName` | Reference Name | string |  |  |  |  |
| `key` | key | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `webapp` |  | object |  |  |  |  |
| `webapp.id` | Internal identifier | string |  |  |  |  |
| `webapp.refName` | Reference Name | string |  |  |  |  |

## webSite-fieldsetCollection

Browser definition `webSite-fieldsetCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | webSite-fieldsetElement[] |  |  | [`webSite-fieldsetElement`](#website-fieldsetelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## webSite-fieldsetElement

Browser definition `webSite-fieldsetElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `fieldSetFields` | Fields Included in Field Set | string |  |  |  |  |
| `fieldSetId` | Field Set ID | string |  |  |  |  |
| `fieldSetName` | Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nKey` | nkey | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## webSiteCollection

Browser definition `webSiteCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | webSite[] |  |  | [`webSite`](#website) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## webSiteSelectOptions

Browser definition `webSiteSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `cartDisplayOrder` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cartUpsellItems` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `categoryListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ccFormTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `checkoutErrorEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `colorSet` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cookiePolicy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `custromeRegistrationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultCustomerCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultHostingRoot` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultShippingMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `downloadAvailableEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `font` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `giftCertificateConfEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `giftCertificateEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `igniteEdition` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `invoiceFormTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemTemplateAccountingtItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemTemplateInformationItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `licenseCodeEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `onlinePriceLevel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderApprovedConfEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderCancelledConfEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderFulfilledConfEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderReceivedConfEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `passwordRecoveryEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentProcessingProfiles` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `registrationConfEmail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `relatedItemsLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesOrderType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `scriptTemplateCreditCard` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `scriptTemplateInvoice` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchCategoryListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchFormItemListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchItemListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchLinkForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `searchPortletForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sitePortletStyle` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteTabAlignment` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteTabStyle` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `upsellItems` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `upsellItemsLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `websiteLogo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `websiteLogoAlign` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `websiteScope` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `websiteTheme` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `webstoreAddItemBehavior` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
