---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768818"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>הפעלת הצפנת Bitlocker באמצעות ' כוונון '

 ניתן להשתמש במדיניות הגנה מפני נקודות קצה כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור מכשירי Windows. לקבלת מידע נוסף, ראה [הגדרות Windows 10 (ואילך) כדי להגן על מכשירים באמצעות ' כוונון](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)'.
 
עליך להיות מודע לכך שמכשירים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, שמופעלת ללא היישום של מדיניות MDM. פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן ברירות מחדל נקבעו. עיין בשאלות הנפוצות הבאות לקבלת פרטים נוספים.
 
לקבלת מידע אודות פתרון בעיות ב-bitlocker, ראה [פתרון בעיות במדיניות bitlocker ב-Microsoft intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**שאלות נפוצות**

ש: אילו מהדורות של הצפנת מכשירים של Windows תומכת באמצעות מדיניות הגנה על נקודות קצה?<br>
ת: ההגדרות במדיניות הגנה על נקודות הקצה מתבצעות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). לא כל המהדורות או גירסאות build של Windows תומכות ב-CSP של Bitlocker. <br><br>

ש: כיצד ניתן להפוך את Bitlocker לזמין במכשירים מבלי לדרוש אינטראקציה של משתמשי קצה?<br>
ת: כל עוד הדרישות הנדרשות מראש מתקיימות, ניתן להפוך את Bitlocker "למצב הצפנה שקט" באמצעות המנגינה. עיין בפרטים של דרישות ההתקן והגדרות מדיניות לדוגמה כדי לאפשר הצפנה שקטה במסמך הבא: [הפיכת הצפנת Bitlocker לזמינה בצורה שקטה](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה ועוצמת הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?<br>
תשובה: לא. כדי להחיל את הגדרות הצופן החדשות, תחילה יש לפענח את הכונן.<br><br>
**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכת מדיניות ההגדרה, המאפשרת שימוש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.
 
ש: אם התקן מוצפן כתוצאה מתוך היישום של מדיניות ה-intune, האם היא תפענח כאשר מדיניות זו תוסר?<br>
ת: הסרת מדיניות הקשורה להצפנה אינה מביאה לפענוח של הכוננים שתצורתם נקבעה.
 
ש: מדוע מדיניות התאימות מציגה כי המכשיר שלי אינו מופעל על-ידי Bitlocker, למרות שהוא מופעל?<br>
ת: ההגדרה "Bitlocker enabled" במדיניות התאימות של ' שימוש בעידון ' משתמשת בלקוח תקינות התקן של Attestation (DHA). לקוח זה מודד רק את מצב ההתקן בזמן האתחול. אז אם התקן לא אותחל מחדש מאז השלמת הצפנת Bitlocker, שירות הלקוח של DHA לא ידווח על Bitlocker כפעיל.
 
 