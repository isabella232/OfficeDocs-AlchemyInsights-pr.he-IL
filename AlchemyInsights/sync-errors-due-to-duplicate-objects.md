---
title: 902 (שגיאות סינכרון עקב אובייקטים כפולים)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708063"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>שגיאות סינכרון עקב אובייקטים כפולים

ייתכן שתקבל אחת מהודעות השגיאה הבאות כאשר סינכרון מדריכי כתובות מסתיים ב-Microsoft 365:

- לא ניתן לעדכן אובייקט זה ב-Microsoft Online Services מאחר שהתכונות הבאות המשויכות לאובייקט זה מכילים ערכים שכבר משויכים לאובייקט אחר במדריך הכתובות המקומי שלך.

- אובייקט מסונכרן עם אותה כתובת proxy קיים כבר במדריך הכתובות של Microsoft Online Services.

- לא ניתן לעדכן אובייקט זה מאחר שהתכונות הבאות המשויכות לאובייקט זה מכילים ערכים שכבר משויכים לאובייקט אחר בשירותי מדריך הכתובות המקומי: UserPrincipalName.

כדי לזהות ולפתור את הבעיה, הורד והפעיל את [כלי התיקון של שגיאות IdFix DirSync](https://github.com/Microsoft/idfix).

לקבלת מידע נוסף, ראה [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
