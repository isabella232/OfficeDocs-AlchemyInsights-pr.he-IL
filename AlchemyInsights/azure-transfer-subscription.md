---
title: העברת בעלות חיובים של Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755548"
---
# <a name="transfer-azure-billing-ownership"></a>העברת בעלות חיובים של Azure

היכנס אל [פורטל Azure](https://portal.azure.com/) כמנהל של חשבון החיוב שכולל את המנוי שברצונך להעביר. אם אינך בטוח אם אתה מנהל, או אם אתה צריך לקבוע מי כן מנהל, ראה [קביעת מנהל חיובים של חשבון](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. חפש _ניהול עלויות + חיוב_.
1. בחר **מנויים** מהחלונית הימנית. בהתאם לגישה, ייתכן שתצטרך לבחור טווח חיובים ולאחר מכן לבחור **מנויים** או **מנויי Azure**.
1. בחר **העברת בעלות של חיובים** עבור המנוי שברצונך להעביר.
1. הזן את כתובת הדואר האלקטרוני של משתמש שהוא מנהל החיובים של החשבון שישמש כבעלים החדש של המנוי ולאחר מכן בחר **שלח בקשת העברה**.
1. המשתמש מקבל הודעות דואר אלקטרוני כולל הוראות לסקירת בקשת ההעברה. כדי לאשר את בקשת ההעברה, המשתמש בוחר את הקישור בהודעת הדואר האלקטרוני ופועל לפי ההוראות.

שים לב שאם אתה מעביר את בעלות החיובים של המנוי שלך לחשבון של משתמש בדייר Azure AD אחר, כל ההקצאות של [בקרת גישה המבוססת על תפקיד (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) לניהול משאבים במנוי יוסרו לצמיתות. רק לבעלים החדש תהיה גישה לניהול משאבים במנוי. לקבלת מידע נוסף אודות האופן שבו ניתן לשנות את מדריך הכתובות עבור מנוי, ראה [העברת מנוי למשתמש בדייר Azure AD אחר](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**השפעה חשובה על החשבוניות שלך**_: אם העברת בעלות חיוב עבור מנויי Azure, החיובים שלך יהיו מדורגים לחיוב. תוכל לגשת לחשבוניות בהתאם לפעולות הבאות:  

1. בחר את המנוי שלך מתוך  [דף המנויים](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) בפורטל Azure בתור [משתמש בעל גישה לחשבוניות](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), לאחר מכן בחר **חשבוניות**.
1. לחץ על **הורד חשבונית** כדי להציג עותק של חשבונית ה- PDF שלך. אם מופיע  _לא זמין_, ראה [מדוע אני לא רואה חשבונית עבור תקופת החיוב האחרונה?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. באפשרותך גם להציג את השימוש היומי שלך על ידי לחיצה על **תקופת חיוב** כדי לקבל קובץ PDF של החשבונית שלך ועותק של קובץ השימוש היומי המפורט שלך (.CSV). לקבלת מידע נוסף, ראה [קבלת חשבונית ונתוני שימוש](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**מסמכים מומלצים**

- [העברת בעליות על חיובים של מנוי Azure לחשבון אחר](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [אודות העברת בעלות חיוב עבור מנוי Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [מנויי פיתוח/בדיקה של העברת Visual Studio,‏רשת השותפים של Microsoft (MPN) ושלם תוך כדי תנועה](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [שאלות נפוצות אודות העברת בעלות](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [פתרון בעיות של העברת בעלות](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
