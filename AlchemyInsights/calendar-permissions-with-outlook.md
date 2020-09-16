---
title: הרשאות לוח שנה
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748794"
---
# <a name="calendar-permissions"></a>הרשאות לוח שנה

משתמשים יכולים לשנות את הרשאות לוח השנה שלהם באמצעות Outlook באינטרנט או לקוחות אחרים, אך כמנהל מערכת, ייתכן שתצטרך גם לחקור אותו.  
באמצעות ה-cmdlet של Exchange PowerShell, תראה את ההרשאה בלוח השנה של המשתמש:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

כדי לראות מידע נוסף, עיין במאמר הבא:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

הרשאות לוח שנה משמשות בשיתוף לוחות שנה, כדי לראות מידע נוסף אודות שיתוף לוח שנה של Outlook, עיין במאמרים הבאים:

- [שיתוף לוח שנה של Outlook עם אנשים אחרים](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [שיתוף לוח השנה שלך ב-Outlook באינטרנט לעסקים](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

כדי לפתור בעיות של הרשאת לוח שנה, באפשרותך להשתמש בכלי [מסייע התמיכה והשחזור](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .