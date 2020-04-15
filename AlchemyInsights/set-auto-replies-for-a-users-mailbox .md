---
title: הגדר תשובות אוטומטיות עבור תיבת דואר של משתמש
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506519"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>הגדר תשובות אוטומטיות עבור תיבת דואר של משתמש

**שיטה 1**

1. היכנס לפורטל של Office 365.

2. עבור אל **משתמשים > משתמשים פעילים** (או **קבוצות > תיבות דואר משותפות** אם תגדיר זאת בתיבת דואר משותפת).

3. בחר משתמש בעל תיבת דואר של Microsoft Exchange.

4. בתפריט הנפתח משמאל, עבור אל **הגדרות דואר > תשובה אוטומטית** (אם מדובר בתיבת דואר משותפת, פשוט לחץ על **תשובות אוטומטיות** במעוף החוצה).

**שיטה 2**

1. היכנס לפורטל הניהול של Office 365 באמצעות אישורי מנהל המערכת.

2. הרחב את **מרכזי הניהול**, ולאחר מכן לחץ על **Exchange**.

3. לחץ על התמונה בפינה העליונה שמאלית, לחץ על **משתמש אחר** ולאחר מכן בחר את תיבת הדואר של המשתמש שברצונך לשנות.

4. בצד ימין, בחר **אפשרויות**, לחץ על **ארגן את הדואר האלקטרוני**, ולאחר מכן לחץ **תשובות אוטומטיות.**

**שיטה 3**

הפעל את ה- cmdlet הבא ב- Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

לקבל מידע נוסף אודות cmdlet זה, ראה [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
