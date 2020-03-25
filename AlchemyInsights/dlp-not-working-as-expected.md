---
title: DLP לא פועלת כמצופה
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932623"
---
# <a name="dlp-not-working-as-expected"></a>DLP לא פועלת כמצופה

**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע. אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי. במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.

לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול. אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה. עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.

 **הגדרת טכנולוגיית DLP**

האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** ב-Office 365 לא פועל כצפוי? אם כן, ודא **שמדיניות** ה-dlp שלך מוגדרת כראוי ושהנתונים שלך מכילים את המידע **שמדיניות dlp** מחפשת בעת חישובו.
  
מדיניות DLP מאפשרת לך לזהות ולהגן על מידע רגיש בארגון שלך. כדי להגדיר את מדיניות DLP, השתמש במידע [הנמצא כאן](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **מה מדיניות DLP מחפשת**
  
בעת שימוש **בסוגי המידע הרגישים המובנים** במרכז האבטחה והתאימות של Office 365, מדיניות DLP מחפשת תבניות ורכיבים ספציפיים בעת זיהוי סוגים רגישים אלה.
  
- **סוגי מידע רגישים מוכללים**

    לקבלת מידע אודות הסוגים המובנים המוכללים ומדיניות DLP מחפשת בעת זיהוי הסוג הרגיש, ראה: [מה מחפשים סוגי המידע הרגישים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **סוגי מידע רגישים מותאמים אישית**

    אם אתה מנסה ליצור סוגי מידע רגישים מותאמים אישית, השתמש במאמר הבא לקבלת מידע אודות אופן יצירת סוג רגיש מותאם אישית: [יצירת סוג מידע רגיש מותאם אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**בדיקת מדיניות DLP**

כדי לבדוק את הנתונים שלך באמצעות סוג מידע מובנה או רגיש מותאם אישית, השתמש באפשרות **סוג מבחן** תחת**סוגי מידע רגישים** **לסיווגים** > . לקבלת מידע נוסף, ראה [בדיקת סוגי מידע רגישים מותאמים אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **דוחות**
  
- קבל תובנות מידע רגישות עם [דוחות DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- ראה פרטים ספציפיים על האירוע עם [דוח אירוע](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
