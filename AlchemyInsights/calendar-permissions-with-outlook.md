---
title: הרשאות לוח שנה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862094"
---
# <a name="calendar-permissions"></a>הרשאות לוח שנה

משתמשים יכולים לשנות את הרשאות לוח השנה שלהם עם Outlook באינטרנט או לקוחות אחרים, אך כמנהל ייתכן שיהיה עליך לחקור גם כן.  
ב-cmdlet של Exchange PowerShell יציג את ההרשאה בלוח השנה של המשתמש:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

כדי לראות מידע נוסף, עיין בפרטים הבאים:

- [הרשאת קבלת-Mailboxbox](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [הרשאת הגדרת דואר אלקטרוני](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [הרשאת הוספת בתיבת דואר](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

הרשאות לוח שנה משמשות בשיתוף לוחות שנה, כדי לראות מידע נוסף אודות שיתוף לוח שנה של Outlook, עיין במאמרים אלה:

- [שיתוף לוח שנה של Outlook עם אנשים אחרים](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [שיתוף לוח השנה שלך ב-Outlook באינטרנט עבור עסקים](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

כדי לפתור בעיות בהרשאת לוח שנה, באפשרותך להשתמש בכלי [מסייע התמיכה והשחזור](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .