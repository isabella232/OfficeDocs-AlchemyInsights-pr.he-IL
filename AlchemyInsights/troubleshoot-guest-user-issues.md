---
title: פתרון בעיות של משתמשים אורחים
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901168"
---
# <a name="troubleshoot-guest-user-issues"></a>פתרון בעיות של משתמשים אורחים

1. לקבלת הדרכה לגבי ניהול גישת אורח ליישומים, ראה [ניהול גישת אורח עם חוות דעת של הודעות מיידיות](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)ב-תכלת.
1. [הוסף משתמשים אורחים למדריך הכתובות בפורטל התכלת](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): בתחלה זה, תוסיף משתמש אורח חדש למדריך הכתובות של "תכלת" באמצעות פורטל התכלת, שלח הזמנה וראה כיצד נראה תהליך החזרת ההזמנה של המשתמש אורח.
1. [הוסף משתמש אורח עם PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): בתחלה זה, תשתמש בפקודה New-AzureADMSInvitation כדי להוסיף משתמש אורח אחד לדייר התכלת.
1. כדי ללמוד כיצד להקצות משתמשים וקבוצות, ליישומים ארגוניים ב-תכלת Active Directory (תכלת לספירה), מתוך הפורטל ' תכלת ' או באמצעות PowerShell, ראה [ניהול הקצאת משתמשים עבור יישום ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. שיתוף פעולה B2B של תכלת (תכלת לספירה) עובד עם רוב היישומים המשולבים באמצעות תכלת לספירה. במאמר [](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)זה, אנו מתרגלים לקבלת הוראות לקביעת התצורה של יישומים פופולריים של SaaS לשימוש עם ' תכלת AD B2B '.
1. כארגון המשתמש ביכולות שיתוף פעולה של שיתוף פעולה של ' תכלת Active Directory ' (תכלת לספירה) להזמנת משתמשים אורחים מארגונים שותפים למודעת התכלת שלך, כעת תוכל לספק למשתמשי B2B אלה גישה ליישומים מקומיים. יישומים מקומיים אלה יכולים להשתמש באימות מבוסס-SAML או באימות משולב של Windows (של יווה) עם הקצאה מוגבלת של Kerberos (KCD). לקבלת מידע נוסף, ראה [הענקת משתמשי B2B ב-תכלת AD access ליישומים המקומיים שלך](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. למד כיצד [להעניק לחשבונות שותפים המנוהלים באופן מקומי גישה למשאבי ענן באמצעות שיתוף פעולה של שיתוף פעולה של "תכלת AD](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)