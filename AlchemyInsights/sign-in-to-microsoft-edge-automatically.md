---
title: היכנס ל- Microsoft Edge באופן אוטומטי
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050695"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>היכנס ל- Microsoft Edge באופן אוטומטי

Microsoft Edge משתמש בחשבון ברירת המחדל של מערכת ההפעלה כדי להיכנס באופן אוטומטי למשתמש בהתאם לתצורה של המכשיר של המשתמש. 

התרחישים של כל סוג של תצורת מכשיר ותהליך הכניסה של המשתמש התלוי שלו מתוארים להלן:

- **ההתקן הוא היברידי/AAD-J:** אפשרות זו זמינה בגירסאות Windows 10, ברמה Windows נמוכה וגירסאות שרת תואמות. המשתמשים מחוברים באופן אוטומטי באמצעות חשבונות Azure Active Directory (AD).
- **המכשיר מצורף לתחום**: אפשרות זו זמינה בגירסאות Windows 10, ברמה Windows וגירסאות שרת תואמות. כברירת מחדל, משתמשים בעלי חשבונות תחום אינם מחוברים באופן אוטומטי; כדי להפוך כניסה אוטומטית לזמינה עבורם, השתמש במדיניות **ConfigureOnPremisesAccountAutoSignIn.** כדי להפוך כניסה אוטומטית לזמינה עבור משתמשים בעלי חשבונות Azure AD, שקול להצטרף באופן היברידי למכשירים שלהם.
- **חשבון ברירת** המחדל של מערכת ההפעלה הוא חשבון Microsoft : אפשרות זו זמינה ב- Windows 10 RS3 (גירסה 1709, גירסת Build מס' 10.0.16299) וגירסאות מתקדמות יותר. לא סביר שהתרחיש יתרחש במכשירים ארגוניים. עם זאת, אם חשבון ברירת המחדל של מערכת ההפעלה הוא חשבון Microsoft, Microsoft Edge להיכנס באופן אוטומטי למשתמש באמצעות חשבון Microsoft.
 
 
