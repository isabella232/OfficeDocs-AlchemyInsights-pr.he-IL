---
title: דוחות יומן ביקורת קלאסיים של SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662209"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>יומני ביקורת של SharePoint ו-OneDrive

## <a name="sharepoint-classic-audit-logs"></a>יומני ביקורת קלאסיים של SharePoint

ביקורת מדור קודם של SPO הועברה ליומן ביקורת מאוחד (רע מ). כל דוחות הביקורת המורשית של SPO מופעלים כעת באמצעות רע מ, והאיתותים של ביקורת מדור קודם הועברו ל-רע מ.

שינויים במפתח:

* חיתוך אינו זמין כיכולת.
* בחירת אירועים ספציפיים לביקורת אינה זמינה. עיין [במסמך זה](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) לקבלת רשימה מלאה של אירועים הניתנים לביקורת כברירת מחדל.
* האפשרות **מיקום** תחת **דוחות מותאמים אישית** אינה זמינה.
* האפשרות **פתיחה או הורדה של אירועים מסמכים** אינה זמינה.

[קביעת תצורה של הגדרות ביקורת עבור אוסף אתרים](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>יומני ביקורת מאוחדים של SharePoint ו-OneDrive מודרניים מתאימות

* [הפעלה/ביטול של רישום ביקורת מאוחדת](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

אין צורך בקביעת תצורה נוספת בתוך SharePoint או ב-OneDrive.

השתמש בחיפוש רישום ביקורת כדי לבדוק את הפעילות של הקבצים, התיקיות, המשתמשים, המשתמשים או ההרשאות:

* [פעילויות קובץ ועמוד](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [פעילויות תיקיה](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [פעילויות בקשת שיתוף וגישה](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [פעילויות סינכרון](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [פעילויות ניהול אתר](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

לקבלת מידע נוסף אודות אופן האחזור של אירועים אלה, ראה [חיפוש ביומן הביקורת](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
