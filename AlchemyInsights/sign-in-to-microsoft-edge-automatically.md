---
title: כניסה ל-Microsoft Edge באופן אוטומטי
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677764"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>כניסה ל-Microsoft Edge באופן אוטומטי

Microsoft Edge משתמש בחשבון ברירת המחדל של מערכת ההפעלה כדי להיכנס באופן אוטומטי למשתמש בהתאם לאופן קביעת התצורה של התקן המשתמש. 

התרחישים של כל סוג של תצורת התקן ותהליך הכניסה של המשתמש התלוי שלו מתוארים להלן:

1. **המכשיר הוא היברידי/עמ-בתים**: אפשרות זו זמינה ב-windows 10, windows ברמה התקדמת וגירסאות שרת מתאימות. משתמשים נכנסו באופן אוטומטי באמצעות חשבונות ה-Active Directory של Active Directory (AD).
2. **המכשיר מצורף לתחום**: אפשרות זו זמינה ב-windows 10, windows ברמה התקדמת וגירסאות שרת מתאימות. כברירת מחדל, משתמשים בעלי חשבונות תחום אינם מוצגים באופן אוטומטי; כדי להפוך את הכניסה האוטומטית לזמינה עבורם, השתמש במדיניות **ConfigureOnPremisesAccountAutoSignIn** . כדי להפוך כניסה אוטומטית לזמינה עבור משתמשים בעלי חשבונות של תכלת לספירה, שקול להצטרף למכשירים שלהם.
3. **חשבון ברירת המחדל של מערכת ההפעלה הוא חשבון Microsoft**: אפשרות זו זמינה ב-WINDOWS 10 RS3 (גירסה 1709, build 10.0.16299) וגירסאות מתקדמות יותר. התרחיש אינו סביר להתרחש במכשירים ארגוניים. עם זאת, אם חשבון ברירת המחדל של מערכת ההפעלה הוא חשבון Microsoft, Microsoft Edge ייכנס באופן אוטומטי למשתמש באמצעות חשבון Microsoft.
 
 
