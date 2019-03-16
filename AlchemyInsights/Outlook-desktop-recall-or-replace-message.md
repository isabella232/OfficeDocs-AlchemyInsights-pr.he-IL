---
title: האחזור בשולחן העבודה של outlook או החלפה הודעת דואר אלקטרוני
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657045"
---
# <a name="recall-or-replace-an-email-message"></a>אחזור או החלפה של הודעת דואר אלקטרוני

- כמנהל מערכת, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**. אין אפשרות לאחזר הודעות ממרכז admin.
- באפשרותך **רק הודעות האחזור אשר נשלחות לאנשים בארגון שלך**. אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אתה זוכר אותו.
- באפשרותך **רק הודעות האחזור שנשלחו מ- Outlook 2016 במחשב**. אם משתמש שולח הודעה באמצעות Outlook עבור Mac או ב- Outlook באינטרנט, אין אפשרות לאחזר אותה.

אחזור או החלפה של הודעת דואר אלקטרוני:

1. בחלונית התיקיות בצד ימין של חלון Outlook, בחר את התיקיה פריטים שנשלחו.
1. לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.
1. בחר את הכרטיסיה **הודעה** ולאחר מכן בחר **פעולות** > **אחזור הודעה זו**.
1. בחר **למחוק עותקים שלא נקראו של הודעה זו** או **למחוק עותקים שלא נקראו ולהחליף בהודעה חדשה**, ולאחר מכן בחר **אישור**.
1. אם אתה שולח הודעה חלופי, חבר את ההודעה ולאחר מכן בחר **לשלוח**.
1. ההצלחה או הכשלון של אחזור הודעה תלוי בהגדרות של הנמען ב- Outlook. עבור השלבים לבדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך

- אם אינך מנהל כללי, יש להוסיף את החשבון שלך תפקיד מנהל גילוי אלקטרוני או תפקיד ניהול תאימות חיפוש כדי לחפש הודעות. כדי למחוק הודעות, תצטרך להצטרף לקבוצה תפקיד ניהול הארגון או תפקיד ניהול חיפוש ומחק לצמיתות. הרשאות עבור תפקידים אלה מוקצות ב [מרכז האבטחה והתאימות](https://go.microsoft.com/fwlink/?linkid=2083731).
- [צור תוכן החיפוש](https://docs.microsoft.com/office365/securitycompliance/content-search) כדי למצוא את ההודעה כדי למחוק.
- [להתחבר PowerShell מרכז תאימות ואבטחה](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

אם אתה משתמש אימות מגורמים רבים, ראה [התחברות אל Office 365 אבטחה ו- PowerShell מרכז תאימות באמצעות אימות מגורמים רבים](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).