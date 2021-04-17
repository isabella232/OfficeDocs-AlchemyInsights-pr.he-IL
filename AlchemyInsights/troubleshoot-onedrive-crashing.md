---
title: פתרון בעיות של קריסות ב- OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826200"
---
# <a name="troubleshoot-onedrive-crashes"></a>פתרון בעיות של קריסות ב- OneDrive

אם OneDrive קורס שוב ושוב, נסה את השלבים הבאים לפתרון בעיות:

**ודא שמפתחות הרישום אינם מוגדרים:**

1. באמצעות עורך הרישום, נווט אל HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. אם DisableFileSyncNGSC קיים ומוגדר ל- 1, פתח את המפתח ושנה את הערך ל- 0.
3. הפעל את OneDrive באופן ידני על-ידי מעבר אל התחל ![הקש על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על אפליקציית שולחן העבודה של OneDrive.

**איפוס OneDrive:**

הערות:

- איפוס OneDrive מנתק את כל חיבורי הסינכרון הקיימים שלך (כולל OneDrive האישי שלך אם הוגדר).
- לא תאבד קבצים או נתונים על-ידי איפוס OneDrive במחשב שלך.

**כדי לאפס את OneDrive:**

1. פתח תיבת דו-שיח הפעלה על-ידי הקשה על מקש Windows ו- R.
2. הקלד %localappdata%\Microsoft\OneDrive\onedrive.exe /reset והקש OK. חלון פקודה עשוי להופיע לזמן קצר.
3. הפעל את OneDrive באופן ידני על-ידי מעבר אל התחל ![הקש על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על אפליקציית שולחן העבודה של OneDrive.

הערות:

- אם בחרת לסנכרן רק כמה תיקיות לפני האיפוס, יהיה עליך לעשות זאת שוב לאחר השלמת הסינכרון. קרא [בחר אילו תיקיות OneDrive לסנכרן עם המחשב שלך](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)לקבלת מידע   נוסף.
- יהיה עליך להשלים פעולה זו עבור OneDrive ו- OneDrive for Business האישיים שלך.