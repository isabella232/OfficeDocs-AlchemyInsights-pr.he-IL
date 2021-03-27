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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398730"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>היכנס ל- Microsoft Edge באופן אוטומטי

Microsoft Edge משתמש בחשבון ברירת המחדל של מערכת ההפעלה כדי להיכנס באופן אוטומטי למשתמש בהתאם לתצורה של המכשיר של המשתמש. 

התרחישים של כל סוג של תצורת מכשיר ותהליך הכניסה של המשתמש התלוי שלו מתוארים להלן:

- **המכשיר הוא היברידי/AAD-J:** אפשרות זו זמינה ב- Windows 10, ב- Windows ברמה נמוכה ובגרסאות שרת תואמות. המשתמשים מחוברים באופן אוטומטי באמצעות חשבונות Azure Active Directory (AD).
- **המכשיר מצורף לתחום**: אפשרות זו זמינה ב- Windows 10, ב- Windows ברמה נמוכה ובגרסאות שרת תואמות. כברירת מחדל, משתמשים בעלי חשבונות תחום אינם מחוברים באופן אוטומטי; כדי להפוך כניסה אוטומטית לזמינה עבורם, השתמש במדיניות **ConfigureOnPremisesAccountAutoSignIn.** כדי להפוך כניסה אוטומטית לזמינה עבור משתמשים בעלי חשבונות Azure AD, שקול להצטרף באופן היברידי למכשירים שלהם.
- **חשבון ברירת** המחדל של מערכת ההפעלה הוא חשבון Microsoft : אפשרות זו זמינה ב- Windows 10 RS3 (גירסה 1709, גירסת Build מס' 10.0.16299) וגירסאות מתקדמות יותר. לא סביר שהתרחיש יתרחש במכשירים ארגוניים. עם זאת, אם חשבון ברירת המחדל של מערכת ההפעלה הוא חשבון Microsoft, Microsoft Edge יחתום באופן אוטומטי על המשתמש באמצעות חשבון Microsoft.
 
 
