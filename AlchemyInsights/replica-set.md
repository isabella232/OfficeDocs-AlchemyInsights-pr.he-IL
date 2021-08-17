---
title: קבוצת עותקים משוכפלים
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110681"
---
# <a name="replica-set"></a>קבוצת עותקים משוכפלים

AADDS נקרא גם כתחום המנוהל. למעשה, שני בקרי תחום זמינים ונשמרים על-ידי הקצה האחורי. שני בקרי התחום כוללים DC ראשי אחד ו- DC אחד של שכפול. גיבויים ב- AADDS (תחום מנוהל) הם תהליך אוטומטי המנוהל על-ידי פלטפורמת Azure. במקרה של בעיה בתחום המנוהל שלך, תמיכה ב- Azure יכולה לסייע לך שחזור מהגיבוי.

אתה יוצר כל ערכת עותקים משוכפלים ברשת וירטואלית. יש להציץ לכל רשת וירטואלית אחרת שמארחת קבוצת עותקים משוכפלים של תחום מנוהל. תצורה זו יוצרת טופולוגיית רשת שינוי התומכת בשכפול מדריכי כתובות. רשת וירטואלית יכולה לתמוך בערכות עותקים משוכפלים מרובים, בתנאי שכל קבוצת עותקים משוכפלים נמצאת ברשת משנה וירטואלית אחרת.

לקבלת פרטים נוספים על קבוצת עותקים משוכפלים, ראה [ערכות עותקים משוכפלים של מושגים.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
