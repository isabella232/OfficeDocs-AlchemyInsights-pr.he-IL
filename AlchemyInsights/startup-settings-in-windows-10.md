---
title: הגדרות אתחול ב-Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751136"
---
# <a name="startup-settings-in-windows-10"></a>הגדרות אתחול ב-Windows 10

**שינוי היישומים הפועלים באופן אוטומטי בעת האתחול**

1. עבור אל [הגדרות _GT_ Apps _GT_ Startup](ms-settings:startupapps?activationSource=GetHelp).

2. ודא שכל יישום שברצונך להפעיל בעת ההפעלה מופעל **.**

**הוספת יישום להפעלה אוטומטית בעת האתחול**

1. לחץ או הקש על **התחל** ואתר את היישום שברצונך להפעיל בעת האתחול.

2. לחץ באמצעות לחצן העכבר הימני על האפליקציה, לחץ על **עוד**ולאחר מכן לחץ על **פתח מיקום קובץ**. פעולה זו פותחת את המיקום שבו נשמר קיצור הדרך ליישום. אם אין אפשרות לפתוח את מיקום הקובץ, משמעות הדבר היא שהיישום אינו יכול לפעול בעת האתחול.

3. כאשר מיקום הקובץ פתוח, הקש על **מקש סמל Windows + R**, הקלד **shell: startup**ולאחר מכן לחץ על **אישור**. פעולה זו פותחת את תיקיית ההפעלה.

4. העתק והדבק את קיצור הדרך לאפליקציה ממיקום הקובץ לתיקיית האתחול.

**אפשרויות אתחול מתקדמות (כולל מצב בטוח, הגדרות UEFI ואתחול ממכשיר אחר)**

1. שמור את עבודתך וסגור את כל המסמכים הפתוחים, מאחר ששלבים אלה יפעילו מחדש את המחשב.

2. עבור אל [הגדרות _GT_ Update _AMP_ Security _GT_ Recovery](ms-settings:recovery?activationSource=GetHelp).

3. תחת **הפעלה מתקדמת**, לחץ על **הפעל מחדש כעת**. 

4. לאחר שהמחשב יופעל מחדש במסך בחר אפשרות:

    - כדי לאתחל ממכשיר כגון כונן USB, לחץ על **השתמש במכשיר**.

    - כדי להזין את הגדרות ה-UEFI (הנקראות לעתים הגדרת BIOS), לחץ על **פתרון בעיות > אפשרויות מתקדמות > הגדרות קושחה של UEFI**. 

    - כדי להיכנס למצב בטוח או לשנות הגדרות אתחול מתקדמות, לחץ על **פתור בעיות > אפשרויות מתקדמות > הגדרות אתחול**ולאחר מכן לחץ על **הפעל מחדש**. ייתכן שתתבקש להזין את [מפתח השחזור של BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). לאחר שהמחשב יופעל מחדש שוב, לחץ על הגדרת האתחול שבה ברצונך להשתמש.