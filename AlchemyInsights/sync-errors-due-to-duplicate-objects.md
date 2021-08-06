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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998795"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>שגיאות סינכרון עקב אובייקטים כפולים

ייתכן שתקבל אחת מהודעות השגיאה הבאות כאשר סינכרון מדריכי כתובות יסיים Microsoft 365:

- אין אפשרות לעדכן אובייקט זה ב- Microsoft Online Services מאחר שהתכונות הבאות המשויכות לאובייקט זה כוללות ערכים שעשויים להיות משויכים כבר לאובייקט אחר במדריך הכתובות המקומי שלך.

- אובייקט מסונכרן עם אותה כתובת Proxy כבר קיים במדריך הכתובות של Microsoft Online Services.

- אין אפשרות לעדכן אובייקט זה מאחר שהתכונות הבאות המשויכות לאובייקט זה כוללות ערכים שעשויים להיות משויכים כבר לאובייקט אחר בשירותים המקומיים שלך: UserPrincipalName.

כדי לזהות ולפתור את הבעיה, הורד ולהפעיל את כלי תיקון השגיאות [IdFix DirSync](https://github.com/Microsoft/idfix).

לקבלת מידע נוסף, [ראה KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
