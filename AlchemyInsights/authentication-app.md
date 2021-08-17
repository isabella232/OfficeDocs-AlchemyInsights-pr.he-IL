---
title: יישום אימות
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082943"
---
# <a name="authentication-app"></a>יישום אימות

אם אתה מנהל מערכת כללי, תוכל לגלות במהירות מה קרה או לאבחן בעיות הקשורות להכניסה של המשתמש באמצעות אבחון [הכניסה.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. הפעל את האבחון על-ידי לחיצה על לחצן "[הפעל אבחון](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)". 
1. אתר את האירוע שיש לנתח על-ידי הזנת הפרטים שיש לך לגבי המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.
1. סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואת הפעולות שתוכל לבצע כדי לבצע שינויים, אם יש צורך בשינויים.

**בדוק את התרחיש הרלוונטי:**

1. אם משתמש אינו מקבל הודעת דחיפה באפליקציית Microsoft Authenticator, ודא שהוא אינו מוצג תחת המשתמשים החסומים של MFA כמתואר בחסימה [ובפיתוח חסימת משתמשים.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. אם המשתמש אינו חסום עבור MFA אך אינו מקבל הודעת דחיפה, הוא יכול לפתוח את אפליקציית Microsoft Authenticator, אשר תמשוך את בקשות האישור הממתינות.
1. כשיטת כניסה חלופית, המשתמש יכול גם ללחוץ על היכנס בדרך אחרת ולבחור להשתמש בקוד אימות מהאפליקציה למכשירים ניידים.
1. האפליקציה Microsoft Authenticator היא השיטה הזמינה היחידה עבור משתמשים רבים. [קבל מידע נוסף על ברירות מחדל](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)של אבטחה , [עיין Authenticator שאלות](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) נפוצות לגבי האפליקציה לקבלת שאלות נפוצות ואופן פתרון אותן.
 
**סרטוני וידאו מומלצים**

[כיצד להגדיר את Authenticator App בטלפון חדש (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
