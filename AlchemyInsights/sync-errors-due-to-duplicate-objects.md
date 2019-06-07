---
title: 902 (שגיאות סינכרון עקב אובייקטים כפולים)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757996"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>שגיאות סינכרון עקב שכפול עצמים

ייתכן שתקבל אחת מהודעות השגיאה הבאות בעת סיום סינכרון ספריות:

- אין אפשרות לעדכן אובייקט זה ב- Microsoft Online Services מכיוון התכונות הבאות המשויך לאובייקט זה יש ערכים שייתכן כבר משוייכים לאובייקט אחר בספריה המקומית שלך.

- אובייקט מסונכרן עם אותה כתובת proxy כבר קיים בספריה שלך השירותים המקוונים של Microsoft.

- אין אפשרות לעדכן אובייקט זה מכיוון התכונות הבאות המשויך לאובייקט זה יש ערכים שייתכן כבר משוייכים לאובייקט אחר בשירותי הספריות המקומי שלך: UserPrincipalName.

כדי לזהות ולתקן את הבעיה, להוריד ולהפעיל את [הכלי תיקון שגיאה של DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832).

לקבלת מידע נוסף, ראה [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
