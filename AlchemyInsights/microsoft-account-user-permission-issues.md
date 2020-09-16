---
title: פתרון בעיות-המשתמש לא נמצא במדריך כתובות
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725408"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>פתרון בעיות-המשתמש לא נמצא במדריך כתובות

אם המשתמשים מקבלים הודעת שגיאה "לא ניתן למצוא את המשתמש" במדריך הכתובות, נסה שוב כאשר סוג הבעיה אינו מופיע במדריך הכתובות.

ניתן להשלים את השלבים הבאים כדי לפתור את הבעיה.

- ודא שהחשבון שקיבל את ההזמנה לדואר אלקטרוני הוא אותו חשבון שנעשה בו שימוש כדי להיכנס במועד מאוחר יותר. ודא שהמשתמש משתמש באותו חשבון כדי לקבל את ההזמנה ולהיכנס לאתר. 

לקבלת מידע נוסף, ראה [כיצד לנהל כינויים עבור חשבון Microsoft שלך </a> כדי לנהל את הכניסה של microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- אתר את כל האתרים שבהם המשתמש מקבל את השגיאה. 

הוסף את "/_layouts/15/people.aspx/membershipgroupid = 0" (בתוך המרכאות הכפולות) עד סוף כתובת ה-URL של האתר. 

דוגמה: https://< "contoso">. sharepoint. com/_layouts/15/people.aspx/membershipGroupId = 0.

- בחר את המשתמש מהרשימה.

- לחץ על **הסר הרשאות משתמש** מרצועת הכלים. 
-  הוסף את המשתמש ושלח אותו מחדש למשתמש.

