---
title: פרישה של כלי גילוי אלקטרוני מדור קודם
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727784"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>פרישה של כלי גילוי אלקטרוני מדור קודם

כתוצאה מהפונקציונליות החדשה והמשופרת של גילוי אלקטרוני במרכז התאימות של Microsoft 365, הכלים הבאים של גילוי אלקטרוני ו-commandlet יצאו לגמלאות בחודשים הקרובים:

- [גילוי אלקטרוני](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ומקום במקום מחזיקים](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) במרכז הניהול של Exchange.

- רכיבי ה-cmdlet של Exchange Online PowerShell התומכים בגילוי אלקטרוני ובמיקום מקומי. (רכיבי cmdlet אלה מזוהים באופן קולקטיבי כרכיבי cmdlet *-MailboxSearch.) הדבר כולל את רכיבי ה-cmdlet הבאים:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- ה [-Cmdlet search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) ב-Microsoft Exchange Online PowerShell.
- הפעולות הבאות ב-API של Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [מתקדם גילוי אלקטרוני v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**ציר זמן לפרישה**:
- **התקיימות ב-1 ביולי 2020** לא ניתן עוד ליצור חיפושים וחסימות חדשים, אך באפשרותך לפעול, לערוך ולמחוק חיפושים קיימים באחריותך בלבד. התמיכה של Microsoft אינה תומכת עוד במקום ב-גילוי אלקטרוני & המחזיקה ב-EAC.
    
- ה **-1 באוקטובר 2020** במקום גילוי אלקטרוני & מכיל פונקציונליות ב-EAC ימוקמו במצב קריאה בלבד, כך שתוכל להסיר רק חיפושים וחסימות קיימים.

**לקבלת מידע נוסף, ראה**:

 - [העברת חיפושי גילוי אלקטרוני מדור קודם והחסימות למרכז התאימות של Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [פרישה של כלי גילוי אלקטרוני מדור קודם](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [שאלות נפוצות אודות גילוי אלקטרוני מקומי ומחזיק מקום במקום](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



