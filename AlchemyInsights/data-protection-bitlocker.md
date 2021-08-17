---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118595"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>הפיכת הצפנת Bitlocker לזמין באמצעות Intune

ניתן להשתמש במדיניות Endpoint Protection Intune כדי לקבוע את התצורה של הגדרות ההצפנה של Bitlocker עבור Windows אחרים. לקבלת מידע נוסף, ראה [Windows 10 (ואילך) כדי להגן על מכשירים באמצעות Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

בנוסף למדיניות Endpoint Protection יש גם דוח הצפנה המספק תצוגה מפורטת יותר של מצב ההצפנה עבור מכשירים. ניתן לגשת הדוח זה בפורטל MEM תחת מכשירים **> צג** ולאחר מכן, תחת קביעת **תצורה,** [בחר הצפנה הדוח](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

אם אתה מוצא ש- Bitlocker אינו זמין כצפוי או שהפרופיל המשמש לזמינה של Bitlocker נמצא במצב שגיאה, עיין בהצפנה הדוח כדי להבין טוב יותר מדוע מתרחש אופן הפעולה.

כדי למצוא פרטים לגבי האופן שבו ניתן לפרש את הדוח, כולל ערכי מצב ההצפנה השונים, ראה [ניטור הצפנת מכשיר באמצעות Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

עליך להיות מודע לכך שהתקנים חדשים רבים יותר פועלים Windows 10 בהצפנת Bitlocker אוטומטית, המופעלת ללא היישום של מדיניות MDM. פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן מוגדרות כברירת מחדל. לקבלת פרטים נוספים, עיין בשאלות הנפוצות הבאות.

לקבלת מידע אודות פתרון בעיות ב- bitlocker, [ראה פתרון בעיות במדיניות BitLocker ב- Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**שאלות נפוצות**

ש: אילו מהדורות של Windows תומכות בהצפנה של מכשירים באמצעות Endpoint Protection המדיניות?<br>
ת: ההגדרות ב- Intune Endpoint Protection מדיניות מיושמת באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). לא כל המהדורות או הגרסאות build של Windows תמיכה ב- CSP של Bitlocker. <br><br>

ש: כיצד ניתן להפוך את Bitlocker לזמין במכשירים ללא צורך באינטראקציה של משתמש קצה?<br>
ת: כל עוד התנאים המוקדמים הדרושים יתקינו, ניתן להפוך את Bitlocker לזמין "הצפנה שקטה" באמצעות Intune. עיין בפרטים של דרישות המכשיר והגדרות מדיניות לדוגמה כדי להפוך הצפנה שקטה לזמינה במסמך הבא: [שקט הפוך הצפנת Bitlocker לזמינה.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

ש: אם מכשיר כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת הצפנה וחוזק הצפנה (XTS-AES-128), החלת מדיניות עם הגדרות שונות מפעילה באופן אוטומטי הצפנה מחדש של הכונן עם ההגדרות החדשות?<br>
תשובה: לא. כדי להחיל את הגדרות הצופן החדשות, יש לפענח תחילה את הכונן.<br><br>
**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שמתרחשת במהלך OOBE אינה מופעלת עד להערכה של מדיניות Intune, המאפשרת להשתמש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.
 
ש: אם מכשיר מוצפן כתוצאה מיישום מדיניות Intune, האם הוא יפענח בעת הסרת מדיניות זו?<br>
ת: הסרת מדיניות הקשורה להצפנה אינה כוללת פענוח של הכוננים שתצורתם נקבעה.
 
ש: מדוע מדיניות תאימות Intune מראה שהמכשיר שלי אינו זמין ב- Bitlocker, למרות שהוא זמין?<br>
ת: ההגדרה "Bitlocker enabled" במדיניות תאימות Intune משתמשת בלקוח בדיקת תקינות התקן Windows (DHA). לקוח זה מודד את מצב המכשיר רק בזמן האתחול. לכן, אם לא אותחל מחדש מכשיר מאז השלמת ההצפנה של Bitlocker, שירות לקוח DHA לא הדוח Bitlocker כפעיל.
 
 