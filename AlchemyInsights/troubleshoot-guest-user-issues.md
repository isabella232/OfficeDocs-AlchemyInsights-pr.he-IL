---
title: פתרון בעיות משתמש אורח
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939380"
---
# <a name="troubleshoot-guest-user-issues"></a>פתרון בעיות משתמש אורח

1. לקבלת הנחיות לניהול גישת אורח ליישומים, ראה ניהול גישת [אורח באמצעות ביקורות גישה של Azure AD](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [הוסף משתמשים אורחים למדריך](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)הכתובות שלך בפורטל Azure : בהתפתחות מהירה זו, תוסיף משתמש אורח חדש לספריית Azure AD שלך דרך פורטל Azure, תשלח הזמנה ו תראה איך נראה תהליך המימוש של ההזמנה של המשתמש אורח.
1. [הוסף משתמש אורח עם PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): בתפריט התחלה מהירה זה, תשתמש בפקודה New-AzureADMSInvitation כדי להוסיף משתמש אורח אחד לדייר Azure שלך.
1. כדי ללמוד כיצד להקצות משתמשים וקבוצות ליישומים ארגוניים ב- Azure Active Directory (Azure AD), מתוך פורטל Azure או באמצעות PowerShell, ראה ניהול הקצאת משתמשים עבור יישום [ב- Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. שיתוף פעולה של Azure Active Directory (Azure AD) B2B פועל עם רוב האפליקציות שמשתלבות עם Azure AD. במאמר [זה,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)אנו עוברים על ההוראות לקביעת התצורה של כמה יישומי SaaS פופולריים לשימוש עם Azure AD B2B.
1. כארגון המשתמש ביכולות שיתוף פעולה של Azure Active Directory (Azure AD) B2B כדי להזמין משתמשים אורחים מארגונים שותפים ל- Azure AD שלך, באפשרותך כעת לספק למשתמשי B2B אלה גישה ליישומים מקומיים. אפליקציות מקומיות אלה יכולות להשתמש באימות מבוסס SAML או באימות Windows משולב (IWA) עם הקצאה מוגבלת של Kerberos (KCD). לקבלת מידע נוסף, ראה [הענק למשתמשי B2B ב- Azure AD גישה ליישומים המקומיים שלך.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. למד כיצד להעניק [לחשבונות שותפים המנוהלים באופן מקומי גישה למשאבי ענן באמצעות שיתוף פעולה של Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).