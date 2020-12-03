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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564620"
---
# <a name="delete-tenant"></a>מחיקת דייר

כדי למחוק מודעה של תכלת, ודא כי:
- אתה מנהל מערכת כללי במדריך הכתובות.
- לא נכנסת באמצעות חשבון בעל מדריך הכתובות המוגדר כברירת מחדל, כגון contoso.onmicrosoft.com בחשבון החתום, כגון admin@contoso.onmicrosoft.com.
- הסר את כל היישומים הפעילים במדריך הכתובות לפני המחיקה. כדי להסיר יישומים פעילים, נווט אל רישומי היישומים והסר את היישומים הקיימים.
- אין מנויים פעילים עבור שירותים מקוונים של Microsoft, כגון Microsoft התכלת, Office 365 או תכלת AD Premium המשויכים למדריך הכתובות. העבר את המנויים שלך או ביטול מזורז של מנויים פעילים באמצעות תמיכה וחיובים של תכלת. קבל מידע נוסף על ביטול מנויים של Office 365 ו-תכלת. לקבלת הנחיות לגבי שיוך או הוספה של מנוי קיים לדייר, ראה [שיוך או הוספה של מנוי תכלת לדייר הודעות תכלת](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- אין רשיון פעיל. כדי להסיר רשיונות, ראה [כיצד להסיר מנוי כדי להסיר את הרשיון](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- אין משתמשים פעילים נוספים במדריך הכתובות מלבד עצמך כמנהל המערכת הכללי כאשר אתה מנסה למחוק את ' תכלת AD '. הסר משתמשים פעילים אחרים, וכל יחסי התלות של שם תחום מותאם אישית בדייר יצטרכו גם הם להסרה, כגון משתמשים שנוצרו באמצעות admin@contoso.com.

לקבלת שלבים נוספים לפירוט:
- מחק את ' תכלת Active Directory ' או ' מנוי ', ראה [מחיקת מדריך כתובות של Active directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- הסרת יישומים במדריך הכתובות, ראה [הסרת יישומים](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
