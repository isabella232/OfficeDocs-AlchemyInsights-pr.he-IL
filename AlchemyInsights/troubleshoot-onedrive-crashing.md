---
title: פתרון בעיות ב-OneDrive קורס
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664999"
---
# <a name="troubleshoot-onedrive-crashes"></a>פתרון בעיות ב-OneDrive קורס

אם OneDrive קורס שוב ושוב, נסה את השלבים הבאים לפתרון בעיות:

**הבטחת מפתחות רישום אינם מוגדרים:**

1. באמצעות עורך הרישום, נווט אל HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. אם DisableFileSyncNGSC מופיע ומוגדר ל-1, פתח את המקש ושנה את הערך ל-0.
3. הפעלה ידנית של OneDrive על-ידי מעבר להתחלה ![הקש על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על יישום שולחן העבודה של OneDrive.

**אפס את OneDrive:**

ערות

- איפוס OneDrive מנתק את כל חיבורי הסינכרון הקיימים (כולל OneDrive האישי שלך, אם הוגדר).
- לא תאבד קבצים או נתונים על-ידי איפוס OneDrive במחשב שלך.

**כדי לאפס את OneDrive:**

1. פתח תיבת דו-שיח של ההפעלה על-ידי הקשה על מקש Windows ו-R.
2. הקלד% localappdata% \Microsoft\OneDrive\onedrive.exe /reset ולחץ על אישור. חלון פקודה עשוי להופיע בקצרה.
3. הפעלה ידנית של OneDrive על-ידי מעבר להתחלה ![הקש על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על יישום שולחן העבודה של OneDrive.

ערות

- אם בחרת לסנכרן רק תיקיות מסוימות לפני האיפוס, יהיה עליך לבצע את הפעולה שוב לאחר השלמת הסינכרון. קרא [בחירת התיקיות של OneDrive שיסונכרנו עם המחשב שלך](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   לקבלת מידע נוסף.
- יהיה עליך להשלים זאת עבור OneDrive האישי וOneDrive for Business.