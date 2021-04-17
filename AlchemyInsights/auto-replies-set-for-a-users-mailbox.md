---
title: הגדר תשובות אוטומטיות עבור תיבת דואר
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
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820935"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>הגדר תשובות אוטומטיות עבור תיבת דואר של משתמש

**שיטה 1**

1. היכנס לפורטל Microsoft 365.

2. עבור אל **משתמשים > משתמשים פעילים** (או **קבוצות > תיבות דואר משותפות** אם תגדיר זאת בתיבת דואר משותפת).

3. בחר משתמש בעל תיבת דואר של Microsoft Exchange.

4. בתפריט הנפתח משמאל, עבור אל **הגדרות דואר > תשובה אוטומטית** (אם מדובר בתיבת דואר משותפת, פשוט לחץ על **תשובות אוטומטיות** במעוף החוצה).

**שיטה 2**

1. היכנס לפורטל הניהול של Microsoft 365 באמצעות אישורי מנהל מערכת.

2. הרחב את **מרכזי הניהול**, ולאחר מכן לחץ על **Exchange**.

3. לחץ על התמונה בפינה העליונה שמאלית, לחץ על **משתמש אחר** ולאחר מכן בחר את תיבת הדואר של המשתמש שברצונך לשנות.

4. בצד ימין, בחר **אפשרויות**, לחץ על **ארגן את הדואר האלקטרוני**, ולאחר מכן לחץ **תשובות אוטומטיות.**

**שיטה 3**

הפעל את ה- cmdlet הבא ב- Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

לקבל מידע נוסף אודות cmdlet זה, ראה [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
