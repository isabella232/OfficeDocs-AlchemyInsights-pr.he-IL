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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932098"
---
# <a name="api-permissions-and-consent"></a>הרשאות API והסכמה

יישומים שמשתלבים עם פלטפורמת הזהויות של Microsoft עוקבים אחר מודל הרשאה המעניק למשתמשים ולמנהלי מערכת שליטה באופן הגישה לנתונים. היישום של מודל ההרשאות עודכן בנקודות פלטפורמת הזהויות של Microsoft קצה. היא משנה את האופן בו יישום חייב לקיים אינטראקציה עם פלטפורמת הזהויות של Microsoft. [הרשאות והסכמה בנקודות פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) מכסה את המושגים הבסיסיים של מודל הרשאה זה, כולל טווחים, הרשאות והסכמה.

מסגרת [ההסכמה של Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) מקלה עליך לפתח יישומי אינטרנט מרובי דיירים ויישומים מקוריים של לקוח. יישומים אלה מאפשרים כניסה על-ידי חשבונות משתמשים מתוך דייר Azure AD השונה מזה שבו היישום רשום. ייתכן שהם עשויים גם לגשת לממשקי API באינטרנט, כגון ה- API של Microsoft Graph (כדי לגשת ל- Azure AD , Intune ולהשירותים ב- Microsoft 365) ולממשקי API שירותי Microsoft אחרים, בנוסף לממשקי API של האינטרנט שלך.

