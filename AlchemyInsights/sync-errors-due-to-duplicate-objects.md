---
title: 902 (שגיאות סינכרון עקב אובייקטים כפולים)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767128"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>שגיאות סינכרון עקב אובייקטים כפולים

ייתכן שתתקבל אחת מהודעות השגיאה הבאות כאשר סינכרון ספריות מסיים ב-Microsoft 365:

- אין אפשרות לעדכן אובייקט זה ב-Microsoft Online Services מאחר שהתכונות הבאות המשויכות לאובייקט זה כוללים ערכים שייתכן שמשויכים כבר לאובייקט אחר בספריה המקומית.

- אובייקט מסונכרן עם אותה כתובת proxy קיים כבר בספריה ' שירותים מקוונים של Microsoft '.

- אין אפשרות לעדכן אובייקט זה מאחר שהתכונות הבאות המשויכות לאובייקט זה כוללים ערכים שייתכן שמשויכים כבר לאובייקט אחר בשירותי הספריה המקומיים שלך: הפקודה Username.

כדי לזהות ולתקן את הבעיה, להוריד ולהפעיל את [כלי תיקון שגיאות Idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

לקבלת מידע נוסף, ראה [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
