---
title: כניסה ל- Windows 10 ללא שימוש בסיסמה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830547"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>כניסה ל- Windows 10 ללא שימוש בסיסמה

כדי להימנע מהקלדה של סיסמה בעת ההפעלה של Windows, מומלץ להשתמש באחת מאפשרויות הכניסה המאובטחות של Windows Hello, כמו מספר זיהוי אישי, זיהוי פנים או טביעת אצבע, אם היא זמינה. אם ברצונך להפוך כניסה מאובטחת ללא זמינה, עיין בהוראות "היכנס באופן אוטומטי ל- Windows 10" להלן.

**Secure Windows Hello חלופות לסיסמאת החשבון**

עבור אל **הגדרות > חשבונות > אפשרויות כניסה** (או לחץ [כאן](ms-settings:signinoptions?activationSource=GetHelp)). אפשרויות הכניסה הזמינות יופיעו ברשימה. לדוגמה:

![אפשרויות כניסה.](media/sign-in-options.png)

לחץ או הקש על אחת מהאפשרויות כדי לקבוע את תצורתה. בפעם הבאה שתפתח או תפתח את Windows, תוכל להשתמש באפשרות החדשה במקום בסיסמה. 

**כניסה אוטומטית ל- Windows 10**

**הערה:** כניסה אוטומטית היא נוחה, אך מציגה סיכון אבטחה, במיוחד אם המחשב שלך נגיש על-ידי אנשים מרובים. 

1. לחץ או הקש על **לחצן** התחל בשורת המשימות.

2. הקלד **netplwiz** ולאחר מכן הקש על מקש Enter כדי לפתוח את החלון חשבונות משתמשים.

3. תחת **חשבונות משתמשים,** לחץ על החשבון שברצונך להיכנס בו באופן אוטומטי בעת הפעלת Windows.

4. בטל את הסימון בתיבת הסימון "משתמשים חייבים להזין שם משתמש וסיסמה כדי להשתמש במחשב זה".

    ![המשתמשים חייבים להזין אפשרות של שם משתמש וסיסמה.](media/users-must-enter-username.png)

5. לחץ על **אישור**. תתבקש להזין ולאשר את הסיסמה עבור החשבון שבחרת. לחץ **על אישור** כדי לסיים. בפעם הבאה ש- Windows 10 יופעל, הוא יירשם באופן אוטומטי לחשבון שבחרת.
