---
title: פתרון בעיות בקריסות של כוננים one
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748920"
---
# <a name="troubleshoot-onedrive-crashes"></a>פתרון בעיות בקריסות של כוננים one

אם OneDrive מתנגש שוב ושוב, נסה את שלבי פתרון התקלות הבאים:

**ודא שמפתחות הרישום אינם מוגדרים:**

1. באמצעות עורך הרישום, נווט אל HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. אם האפשרות Disאייקובלקובץ Syncngsc מוגדרת ל-1, פתח את המפתח ושנה את הערך ל-0.
3. הפעלה ידנית של OneDrive על ידי הולך להתחיל ![לחץ על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), סוג OneDrive בתיבת החיפוש ולאחר מכן לחץ על יישום OneDrive שולחן העבודה.

**אפס כונן OneDrive:**

ערות

- איפוס OneDrive מנתק את כל חיבורי הסינכרון הקיימים (כולל הכונן האישי שלך, אם תגדיר).
- לא תאבד קבצים או נתונים על-ידי איפוס כונן OneDrive במחשב שלך.

**כדי לאפס את כונן OneDrive:**

1. פתח תיבת דו-שיח של הפעלה על-ידי הקשה על מקש Windows ו-R.
2. הקלד% localappdata% \Microsoft\OneDrive\onedrive.exe /איפוס ולחץ על אישור. חלון פקודה עשוי להופיע בקצרה.
3. הפעלה ידנית של OneDrive על ידי הולך להתחיל ![לחץ על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), סוג OneDrive בתיבת החיפוש ולאחר מכן לחץ על יישום OneDrive שולחן העבודה.

ערות

- אם בחרת לסנכרן תיקיות מסוימות בלבד לפני האיפוס, יהיה עליך לעשות זאת שוב לאחר השלמת הסינכרון. קרא [בחר באילו תיקיות OneDrive יש לסנכרן למחשב שלך](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   לקבלת מידע נוסף.
- יהיה עליך להשלים את זה עבור הכונן האישי שלך OneDrive עבור עסקים.