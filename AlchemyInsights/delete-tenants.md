---
title: מחיקת דייר
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993894"
---
# <a name="delete-tenant"></a>מחיקת דייר

כדי למחוק AD של Azure, ודא:
- אתה מנהל מערכת כללי במדריך הכתובות.
- לא נכנסת באמצעות חשבון הכולל את מדריך הכתובות המהווה ברירת contoso.onmicrosoft.com בחשבון החתימה, כגון admin@contoso.onmicrosoft.com.
- הסר יישומים פעילים במדריך הכתובות לפני המחיקה. כדי להסיר יישומים פעילים, נווט אל רישומי יישומים והסר את היישומים הקיימים.
- אין מנויים פעילים עבור שירותים מקוונים של Microsoft, כגון Microsoft Azure, Office 365 או Azure AD Premium המשויכים למדריך הכתובות. העבר את המנויים שלך או זרז את הביטול של מנויים פעילים באמצעות Azure Support and Billing. קבל מידע נוסף על ביטול מנויי Office 365 ו- Azure. לקבלת הנחיות לגבי שיוך או הוספה של מנוי קיים לדייר, ראה שיוך או הוספת מנוי [Azure לדייר Azure AD שלך.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- אין רשיון פעיל. כדי להסיר רשיונות, ראה [כיצד להסיר מנוי להסרת רשיון.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- אין משתמשים פעילים אחרים במדריך הכתובות מלבד עצמך כמנהל המערכת הכללי בעת ניסיון למחוק את Azure AD. הסר את כל המשתמשים הפעילים האחרים, ואת כל יחסי התלות בשם תחום מותאם אישית הדייר יהיה צורך גם להסיר, כגון משתמשים שנוצרו באמצעות admin@contoso.com.

לקבלת שלבים מפורטים יותר לגבי אופן הפעולות הבאות:
- מחק את "Azure Active Directory" או "מנוי", ראה [מחיקת Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- הסרת יישומים במדריך הכתובות, ראה [הסרת יישומים.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
