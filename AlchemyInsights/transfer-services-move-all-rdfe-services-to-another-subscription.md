---
title: שירותי העברה-העברת כל שירותי RDFE למנוי אחר
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692044"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>שירותי העברה-העברת כל שירותי RDFE למנוי אחר

**העברת משאבים**

ניתן להעביר משאבים של תכלת לקבוצת משאבים או לקבוצת משאבים אחרת תחת אותו מנוי באמצעות הפורטל התכלת, התכלת PowerShell, התכלת CLI או ה-API של REST כדי להעביר משאבים.

לפני שתוכל להעביר משאבים, ראה:

- [רשימת פעולות לביצוע לפני העברת משאבים](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [שירותים שניתן להעביר](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [כיצד לאמת את המעבר](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [העברת הדרכה עבור שירותים](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

כדי להעביר משאבים קיימים לקבוצת משאבים או למנוי אחר, באפשרותך להשתמש ב:

- [פורטל תכלת](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [תכלת PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [תכלת CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [מסוף API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

ערכת לימוד: [העברת משאבים של תכלת לקבוצת משאבים או למנוי אחר](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**פתרון שגיאות באמצעות מנהל המשאבים של תכלת**

עיין במאמרים הבאים כדי לקבל מידע על שגיאות משותפות בפריסה של תכלת ולקבל מידע כדי לפתור אותן. אם אינך מצליח למצוא את קוד השגיאה עבור שגיאת הפריסה שלך, ראה [איתור קוד שגיאה](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [פתרון בעיות של שגיאות פריסה](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [פתרון בעיות בהעברת משאבי תכלת לקבוצת משאבים או למנוי חדש](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

שים לב שאם ברצונך לשדרג את מנוי התכלת שלך, כגון מעבר ללא תשלום לתשלום לפי הצורך, יהיה עליך להמיר את המנוי שלך.

- כדי לשדרג גירסת ניסיון ללא תשלום, ראה [שדרוג גירסת הניסיון ללא תשלום או מנוי מתאר התכלת של Microsoft לתשלום לפי-לך](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- כדי לשנות חשבון של תשלום כפי שתרצה, ראה [שינוי המנוי של ' שלמו לפי כשאתה ' להצעה אחרת](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**כדי להוסיף או לשייך מנוי של תכלת לדייר של תכלת Active Directory:**

1. היכנס ובחר את המנוי שבו ברצונך להשתמש [בדף ' מנויים ' בפורטל התכלת](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. בחר **Change directory**.
3. סקור את כל האזהרות שמופיעות ולאחר מכן בחר **שנה**.
4. הספריה משתנה עבור המנוי ותקבל הודעת הצלחה.
5. השתמש בבורר *הספריות* כדי לעבור אל מדריך הכתובות החדש. ייתכן שיחלפו עד 10 דקות עד שהכל יופיע כראוי.

**מסמכים מומלצים**

- [העברת הבעלות על מנוי תכלת](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [העברת משאבים לקבוצת משאבים או למנוי חדש](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [ניהול משאבים באמצעות פורטל תכלת](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
