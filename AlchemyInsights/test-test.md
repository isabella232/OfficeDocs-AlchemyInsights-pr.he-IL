---
title: תנאים חסרים SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106427"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>הפיכת הצפנת Bitlocker לזמין באמצעות Intune

ניתן להשתמש במדיניות Endpoint Protection Intune כדי לקבוע את תצורת הגדרות ההצפנה של Boitlocker עבור מכשירי Windows כמתואר ב: הגדרות Windows10 (ואילך) כדי להגן על מכשירים באמצעות Intune

עליך להיות מודע לכך שהתקנים חדשים רבים יותר פועלים Windows 10 בהצפנת bitlocker אוטומטית המופעלת ללא היישום של מדיניות MDM. פעולה זו עשויה להשפיע על יישום המדיניות אם הגדרות שאינן מוגדרות כברירת מחדל. לקבלת פרטים נוספים, ראה שאלות נפוצות.


שאלות נפוצות ש: אילו מהדורות של Windows תמיכה בהצפנה של מכשירים המשתמשים במדיניות Endpoint Protection שלך?
ת: ההגדרות ב- Intune Endpoint Protection מיושמות באמצעות CSP של Bitlocker.  לא כל המהדורות או הגרסאות build של Windows תומכים ב- CSP של Bitlocker. בשלב זה Windows Editions: Enterprise; החינוך, הנייד, Mobile Enterprise ו- Professional (מ- build מס' 1809 ואילך) נתמכים.




ש: אם מכשיר כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת הצפנה וחוזק הצפנה (XTS-AES-128) יחול מדיניות עם הגדרות שונות באופן אוטומטי מפעיל הצפנה מחדש של הכונן עם ההגדרות החדשות?

תשובה: לא. כדי להחיל את הגדרות הצופן החדשות, יש לפענח תחילה את הכונן.

הערה עבור מכשירים שנרשמו באמצעות Autopilot, ההצפנה האוטומטית שמתרחשת במהלך OOBE אינה מופעלת עד להערכה של מדיניות Intune, המאפשרת להשתמש בהגדרות מבוססות המדיניות במקום ברירות המחדל של מערכת ההפעלה




ש אם מכשיר מוצפן כתוצאה מיישום מדיניות Intune, הוא יפענח בעת הסרת מדיניות זו?

ת: הסרת מדיניות הקשורה להצפנה אינה כוללת פענוח של הכוננים שהוגדרו.




ש: מדוע מדיניות Intune Compliance מראה שהמכשיר שלי אינו "Bitlocker Enabled" אך הוא זמין?

ת: ההגדרה "Bitlocker enabled" במדיניות תאימות intune משתמשת בלקוח בדיקת תקינות התקן Windows (DHA). לקוח זה מודד את מצב המכשיר רק בזמן האתחול. לכן, אם לא אותחל מחדש מכשיר מאז השלמת ההצפנה של bitlocker, שירות לקוח DHA לא הדוח bitlocker כפעיל.