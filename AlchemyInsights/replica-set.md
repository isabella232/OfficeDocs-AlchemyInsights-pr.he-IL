---
title: הקבוצה ' עותק משוכפל '
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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714257"
---
# <a name="replica-set"></a>הקבוצה ' עותק משוכפל '

AADDS נקרא גם התחום המנוהל. למעשה, שני בקרי תחום מופעלים ומתקיימים על-ידי הקצה העורפי. שני DCs כוללים DC ראשי אחד ושכפול אחד DC. גיבויים ב-AADDS (תחום מנוהל) הם תהליך אוטומטי שמנוהל על-ידי פלטפורמת התכלת. במקרה של בעיה בתחום המנוהל שלך, התמיכה בנושא תכלת יכולה לסייע לך בשחזור מהגיבוי.

אתה יוצר כל עותק משוכפל ברשת וירטואלית. כל רשת וירטואלית חייבת להיות מוסדרת לכל רשת וירטואלית אחרת המארחת ערכת עותקים משוכפלים של תחום מנוהל. תצורה זו יוצרת טופולוגיה של רשת שינוי שתומכת בשכפול מדריכי כתובות. רשת וירטואלית יכולה לתמוך בערכות עותק משוכפל מרובות, בתנאי שכל קבוצת עותקים משוכפלים נמצאת ברשת משנה וירטואלית אחרת.

לקבלת פרטים נוספים על קבוצת עותקים משוכפלים, ראה [ערכות עותקים משוכפלים של מושגים](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
