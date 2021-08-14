---
title: העברת שירותים - העברת כל שירותי RDFE למנוי אחר
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940058"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>העברת שירותים - העברת כל שירותי RDFE למנוי אחר

**העברת משאבים**

ניתן להעביר משאבים של Azure למנוי Azure או לקבוצת משאבים אחרת תחת אותו מנוי באמצעות פורטל Azure, Azure PowerShell, Azure CLI או ה- API של REST כדי להעביר משאבים.

כדי שתוכל להעביר משאבים, ראה:

- [רשימת פעולות לביצוע לפני העברת משאבים](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [שירותים הניתנים לתזזה](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [כיצד לאמת את המהלך](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [העברת הדרכה עבור שירותים](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

כדי להעביר משאבים קיימים לקבוצת משאבים אחרת או למנוי אחר, באפשרותך להשתמש:

- [פורטל Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

ערכת לימוד: [העברת משאבי Azure לקבוצת משאבים אחרת או למנוי אחר](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**פתרון בעיות בשגיאות באמצעות Azure Resource Manager**

עיין במאמרים שלהלן כדי ללמוד על כמה שגיאות פריסה נפוצות של Azure ולקבל מידע כדי לפתור אותן. אם אינך מוצא את קוד השגיאה עבור שגיאת הפריסה, ראה [איתור קוד שגיאה](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [פתרון בעיות של שגיאות פריסה](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [פתרון בעיות בהזזת משאבי Azure לקבוצת משאבים חדשה או למנוי חדש](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

שים לב שאם תרצה לשדרג את המנוי שלך ב- Azure, כגון מעבר ללא תשלום ל-pay-as-you-go, יהיה עליך להמיר את המנוי שלך.

- כדי לשדרג גירסת ניסיון ללא תשלום, ראה שדרוג גירסת הניסיון ללא [תשלום או מנוי Microsoft Imagine Azure ל- Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- כדי לשנות חשבון Pay-as-you-go, ראה [שינוי מנוי Azure Pay-As-You-Go להצעה אחרת](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**כדי להוסיף או לשייך מנוי Azure לדייר Azure Active Directory שלך:**

1. היכנס ובחר את המנוי שברצונך להשתמש בו מהדף [מנויים בפורטל Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. בחר **שנה ספריה**.
3. סקור את האזהרות שמופיעות ולאחר מכן בחר **שנה**.
4. מדריך הכתובות משתנה עבור המנוי ואתה מקבל הודעת הצלחה.
5. השתמש *במחליף מדריך* הכתובות כדי לעבור לספריה החדשה שלך. ייתכן ש- 10 דקות לכל דבר יופיעו כראוי.

**מסמכים מומלצים**

- [העברת בעלות על מנוי Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [העברת משאבים לקבוצת משאבים חדשה או למנוי חדש](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [ניהול משאבים באמצעות פורטל Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
