---
title: פתרון בעיות - המשתמש לא נמצא במדריך הכתובות
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098171"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>פתרון בעיות - המשתמש לא נמצא במדריך הכתובות

אם משתמשים מקבלים הודעת שגיאה "אין אפשרות למצוא את המשתמש" במדריך הכתובות, נסה שוב היכן שסוג הבעיה הוא משתמש שלא נמצא במדריך הכתובות.

ניתן להשלים את השלבים הבאים כדי לפתור את הבעיה.

- ודא שהחשבון שקיבלת את ההזמנה לדואר אלקטרוני הוא אותו חשבון המשמש להכניסה מאוחר יותר. ודא שהמשתמש משתמש באותו חשבון כדי לקבל את ההזמנה ולהירשם לאתר. 

לקבלת מידע נוסף, [ראה כיצד לנהל כינויים עבור חשבון Microsoft שלך </a> כדי לנהל את Microsoft 365 הכניסה](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- עבור אל כל אתר שבו המשתמש מקבל את השגיאה. 

הוסף "/_layouts/15/people.aspx/membershipgroupid=0" (בתוך מרכאות כפולות) לסוף כתובת ה- URL של האתר. 

דוגמה: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- בחר את המשתמש מהרשימה.

- לחץ **על הסר הרשאות משתמש** מרצועת הכלים. 
-  הוסף בחזרה את המשתמש ונציג מחדש את ההזמנה למשתמש.

