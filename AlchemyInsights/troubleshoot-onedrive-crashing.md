---
title: פתרון OneDrive קריסות
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921008"
---
# <a name="troubleshoot-onedrive-crashes"></a>פתרון OneDrive קריסות

אם OneDrive קורס שוב ושוב, נסה את השלבים הבאים לפתרון בעיות:

**ודא שמפתחות הרישום אינם מוגדרים:**

1. באמצעות עורך הרישום, נווט אל HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. אם DisableFileSyncNGSC קיים ומוגדר ל- 1, פתח את המפתח ושנה את הערך ל- 0.
3. הפעל את OneDrive באופן ידני על-ידי מעבר אל התחל ![הקש על Windows מקש](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על האפליקציה OneDrive שולחן העבודה.

**אפס OneDrive:**

הערות:

- איפוס OneDrive מנתק את כל חיבורי הסינכרון הקיימים שלך (כולל הסינכרון OneDrive אם הוגדר).
- לא תאבד קבצים או נתונים על-ידי איפוס OneDrive במחשב שלך.

**כדי לאפס OneDrive:**

1. פתח תיבת דו-שיח הפעלה על-ידי Windows על מקש R.
2. הקלד %localappdata%\Microsoft\OneDrive\onedrive.exe /reset והקש OK. חלון פקודה עשוי להופיע לזמן קצר.
3. הפעל את OneDrive באופן ידני על-ידי מעבר אל התחל ![הקש על Windows מקש](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על האפליקציה OneDrive שולחן העבודה.

הערות:

- אם בחרת לסנכרן רק כמה תיקיות לפני האיפוס, יהיה עליך לעשות זאת שוב לאחר השלמת הסינכרון. קרא [בחר אילו OneDrive לסינכרון עם המחשב שלך](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)לקבלת מידע   נוסף.
- יהיה עליך להשלים פעולה זו עבור OneDrive ו- OneDrive for Business.