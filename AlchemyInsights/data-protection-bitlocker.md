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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731240"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>הפעלת הצפנת Bitlocker באמצעות ' כוונון '

 ניתן להשתמש במדיניות הגנה מפני נקודות קצה כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור מכשירי Windows. לקבלת מידע נוסף, ראה [הגדרות Windows 10 (ואילך) כדי להגן על מכשירים באמצעות ' כוונון](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)'.
 
עליך להיות מודע לכך שמכשירים חדשים רבים שבהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, שמופעלת ללא היישום של מדיניות MDM. פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן ברירות מחדל נקבעו. עיין בשאלות הנפוצות הבאות לקבלת פרטים נוספים.
 
לקבלת מידע אודות פתרון בעיות ב-bitlocker, ראה [פתרון בעיות במדיניות bitlocker ב-Microsoft intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**שאלות נפוצות**

 ש: אילו מהדורות של הצפנת מכשירים של Windows תומכת באמצעות מדיניות הגנה על נקודות קצה?<br>
 ת: ההגדרות במדיניות הגנה על נקודות הקצה מתבצעות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). לא כל המהדורות או גירסאות build של Windows תומכות ב-CSP של Bitlocker. <br><br>
      בשלב זה, המהדורות הבאות של Windows נתמכות: Enterprise, השכלה, Mobile, Mobile Enterprise ו-Professional (גירסת build מס ' 1809 ואילך).
 
ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה ועוצמת הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות באופן אוטומטי הפעלת הצפנה מחדש של הכונן עם ההגדרות החדשות?<br>
תשובה: לא. כדי להחיל את הגדרות הצופן החדשות, תחילה יש לפענח את הכונן.<br><br>
**הערה:** עבור מכשירים שנרשמו באמצעות טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכת מדיניות ההגדרה, המאפשרת שימוש בהגדרות המבוססות על מדיניות במקום ברירות המחדל של מערכת ההפעלה.
 
ש: אם התקן מוצפן כתוצאה מתוך היישום של מדיניות ה-intune, האם היא תפענח כאשר מדיניות זו תוסר?<br>
ת: הסרת מדיניות הקשורה להצפנה אינה מביאה לפענוח של הכוננים שתצורתם נקבעה.
 
ש: מדוע מדיניות התאימות מציגה כי המכשיר שלי אינו מופעל על-ידי Bitlocker, למרות שהוא מופעל?<br>
ת: ההגדרה "Bitlocker enabled" במדיניות התאימות של ' שימוש בעידון ' משתמשת בלקוח תקינות התקן של Attestation (DHA). לקוח זה מודד רק את מצב ההתקן בזמן האתחול. אז אם התקן לא אותחל מחדש מאז השלמת הצפנת Bitlocker, שירות הלקוח של DHA לא ידווח על Bitlocker כפעיל.
 
 