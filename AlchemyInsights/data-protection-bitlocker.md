---
title: הגנת נתונים-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908711"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>הפעלת הצפנת Bitlocker עם Intune

 ניתן להשתמש במדיניות הגנת נקודות קצה Intune כדי לקבוע את תצורת הגדרות ההצפנה של Bitlocker עבור התקני Windows. לקבלת מידע נוסף, ראה [הגדרות Windows 10 (וגירסאות מאוחרות יותר) כדי להגן על התקנים באמצעות Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
עליך להיות מודע לכך שהתקנים חדשים רבים בהם פועל Windows 10 תומכים בהצפנת Bitlocker אוטומטית, המופעלת ללא היישום של מדיניות MDM. הדבר עלול להשפיע על יישום המדיניות אם תצורתה של הגדרות שאינן מוגדרות כברירת מחדל נקבעה. לפרטים נוספים, עיין בשאלות הנפוצות הבאות.
 
לקבלת מידע אודות פתרון בעיות [באמצעות bitlocker, ראה פתרון בעיות של מדיניות bitlocker ב-Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**שאלות נפוצות**

 ש: אילו מהדורות של הצפנת התקן של Windows תומכות באמצעות מדיניות הגנת נקודות קצה?<br>
 ת: ההגדרות במדיניות הגנת נקודות קצה Intune מיושמות באמצעות [CSP של Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). לא כל המהדורות או בניית Windows תומכים ב-CSP של Bitlocker. <br><br>
      בשלב זה, המהדורות הבאות של Windows נתמכות: ארגון, חינוך, נייד, מפעל נייד ומקצועי (לבנות 1809 ומעלה).
 
ש: אם התקן כבר מוצפן באמצעות Bitlocker באמצעות הגדרות ברירת המחדל של מערכת ההפעלה עבור שיטת ההצפנה וחוזק הצופן (XTS-AES-128), החלת מדיניות עם הגדרות שונות תפעיל באופן אוטומטי הצפנה מחדש של הכונן עם ההגדרות החדשות?<br>
A: לא. כדי להחיל את הגדרות ההצפנה החדשות, יש לפענח תחילה את הכונן.<br><br>
**הערה:** עבור התקנים הרשומים עם טייס אוטומטי, ההצפנה האוטומטית שתתרחש במהלך OOBE אינה מופעלת עד להערכה של מדיניות Intune, דבר המאפשר להשתמש בהגדרות מבוססות המדיניות במקום ברירות המחדל של מערכת ההפעלה.
 
ש: אם התקן מוצפן כתוצאה מיישום מדיניות Intune, האם הוא יהיה מפוענח בעת הסרת מדיניות זו?<br>
ת: הסרת מדיניות הקשורה להצפנה אינה נובעת מפענוח הכוננים שתצורתם נקבעה.
 
ש: מדוע מדיניות התאימות של Intune מראה שלהתקן שלי אין Bitlocker מאופשר, למרות שהוא?<br>
ת: ההגדרה "Bitlocker מאופשר" במדיניות התאימות Intune מנצלת את לקוח בריאות ההתקנים של Windows (DHA). לקוח זה מודד את מצב ההתקן בזמן האתחול. לכן, אם התקן לא אותחל מההתחלה מאחר שהצפנת Bitlocker הושלמה, שירות לקוח DHA לא ידווח על Bitlocker כפעיל.
 
 