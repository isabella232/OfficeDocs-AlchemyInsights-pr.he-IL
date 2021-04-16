---
title: פרישה של כלי גילוי אלקטרוני מדור קודם
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798550"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>פרישה של כלי גילוי אלקטרוני מדור קודם

כתוצאה מהפונקציונליות החדשה והממשופרת של גילוי אלקטרוני במרכז התאימות של Microsoft 365, הכלים והפקודה הבאים של גילוי אלקטרוני מדור קודם יוצאו משימוש בחודשים הקרובים:

- [גילוי אלקטרוני במקום והמתנה](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) במקום [במרכז](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) הניהול של Exchange.

- כלי ה- cmdlet של PowerShell של Exchange Online התומכים בIn-Place גילוי אלקטרוני In-Place מחזיק. (כלי cmdlet אלה מזוהים יחד כרכיבי cmdlet של *-MailboxSearch.) פעולה זו כוללת את כלי ה- cmdlet הבאים:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) ב- Exchange Online PowerShell.
- הפעולות הבאות ב- API של Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [מתקדם eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**ציר זמן לפרישה**:
- **1 ביולי 2020** לא ניתן עוד ליצור חיפושים והחזקות חדשים, אך באפשרותך להפעיל, לערוך ולמחוק חיפושים קיימים על-פי הסיכון שלך. התמיכה של Microsoft אינה תומכת עוד In-Place גילוי אלקטרוני & ב- EAC.
    
- **1 באוקטובר 2020** In-Place גילוי אלקטרוני & מחזיק פונקציונליות ב- EAC תוצב במצב קריאה בלבד, כך שתוכל להסיר רק חיפושים קיימים והחזקות.

**לקבלת מידע נוסף, ראה**:

 - [העברת חיפושים מדור קודם של גילוי אלקטרוני ונאחזת במרכז התאימות של Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [פרישה של כלי גילוי אלקטרוני מדור קודם](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [שאלות נפוצות In-Place גילוי אלקטרוני In-Place מחזיק](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



