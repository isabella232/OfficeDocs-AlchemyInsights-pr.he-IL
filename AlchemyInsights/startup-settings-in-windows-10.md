---
title: הגדרות אתחול ב- Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909827"
---
# <a name="startup-settings-in-windows-10"></a>הגדרות אתחול ב- Windows 10

**שינוי האפליקציות שפעלו באופן אוטומטי בעת האתחול**

1. עבור אל [הגדרות > יישומים > אתחול](ms-settings:startupapps?activationSource=GetHelp).

2. ודא שכל יישום שברצונך להפעיל בעת האתחול **מופעל**.

**הוספת יישום להפעלה אוטומטית בעת האתחול**

1. לחץ או הקש **על התחל** ומצא את היישום שברצונך להפעיל בעת האתחול.

2. לחץ באמצעות לחצן העכבר הימני על היישום, **לחץ על** עוד ולאחר מכן לחץ על פתח **מיקום קובץ**. פעולה זו פותחת את המיקום שבו קיצור הדרך לאפליקציה נשמר. אם אין אפשרות עבור פתח מיקום קובץ, פירוש הדבר שלא ניתן להפעיל את היישום בעת האתחול.

3. עם מיקום הקובץ פתוח, הקש על **מקש Windows + R**, הקלד **shell:startup** ולאחר מכן לחץ על **אישור.** פעולה זו פותחת את תיקיית האתחול.

4. העתק והדבק את קיצור הדרך לאפליקציה ממיקום הקובץ לתיקיה 'אתחול'.

**אפשרויות אתחול מתקדמות (כולל כספת מצב, הגדרות UEFI ואתחול ממכשיר אחר)**

1. שמור את עבודתך וסגור מסמכים פתוחים, מאחר ששלבים אלה יפעילו מחדש את המחשב.

2. עבור אל [הגדרות > עדכון & אבטחה > שחזור](ms-settings:recovery?activationSource=GetHelp).

3. תחת **אתחול מתקדם**, לחץ על הפעל מחדש **כעת**. 

4. לאחר שהמחשב יופעל מחדש למסך בחר אפשרות:

    - כדי לאתחל ממכשיר, כמו כונן USB, לחץ **על השתמש בהתקן**.

    - כדי להזין את הגדרות ה- UEFI (הנקראות לעתים הגדרת ה- BIOS), **לחץ על פתרון > אפשרויות מתקדמות > קושחה של UEFI הגדרות**. 

    - כדי להיכנס למצב כספת או לשנות הגדרות אתחול מתקדמות, לחץ **על פתרון > אפשרויות מתקדמות > אתחול הגדרות** ולאחר מכן לחץ על הפעל **מחדש.** ייתכן שתתבקש להזין את מפתח השחזור [של BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). לאחר שהמחשב יופעל מחדש שוב, לחץ על הגדרת האתחול שברצונך להשתמש בה.