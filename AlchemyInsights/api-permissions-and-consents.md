---
title: הרשאות API והסכמה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974605"
---
# <a name="api-permissions-and-consent"></a>הרשאות API והסכמה

יישומים המשולבים בפלטפורמת הזהויות של Microsoft ממלאים אחר מודל הרשאה המעניק למשתמשים ולשליטה באופן שבו ניתן לגשת לנתונים. היישום של מודל ההרשאות עודכן בנקודת הקצה של פלטפורמת הזהות של Microsoft. היא משנה את אופן הפעולה של האפליקציה עם פלטפורמת הזהות של Microsoft. [הרשאות והסכמה בנקודת הקצה של פלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) מכסה את המושגים הבסיסיים של מודל הרשאה זה, כולל טווחים, הרשאות והסכמה.

[מסגרת ההסכמה של תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) מאפשרת לך לפתח בקלות יישומי אינטרנט ולקוחות מקוריים של ריבוי דיירים. יישומים אלה מאפשרים כניסה על-ידי חשבונות משתמשים מדייר תכלת לספירה שונה מזה שבו היישום רשום. ייתכן שתצטרך גם לגשת לממשקי Api של אינטרנט, כגון Microsoft Graph API (כדי לגשת אל התכלת לספירה, לכוונן ולשירותים ב-Microsoft 365) וממשקי Api אחרים של Microsoft services, בנוסף לממשקי ה-Api של האינטרנט שלך.

