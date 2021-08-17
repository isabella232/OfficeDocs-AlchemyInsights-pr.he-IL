---
title: הרשאות לוח שנה
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046105"
---
# <a name="calendar-permissions"></a>הרשאות לוח שנה

משתמשים יכולים לשנות הרשאות לוח שנה משלהם עם Outlook באינטרנט או בלקוחות אחרים, אך כמנהל מערכת, ייתכן שתצטרך גם לחקור.  
עם Exchange ה- cmdlet של PowerShell, תראה לך את ההרשאה בלוח השנה של משתמש:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

כדי לראות מידע נוסף, ראה את הפעולות הבאות:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

הרשאות לוח שנה משמשות לשיתוף לוחות שנה, כדי לראות מידע נוסף אודות שיתוף לוח שנה Outlook, עיין במאמרים הבאים:

- [שיתוף לוח שנה של Outlook עם אנשים אחרים](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [שיתוף לוח השנה שלך Outlook באינטרנט לעסקים](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

כדי לפתור בעיות של הרשאת לוח שנה, [באפשרותך להשתמש בכלי מסייע התמיכה והשחזור שלך.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)