---
title: אודות זהות Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918938"
---
# <a name="about-identity-in-yammer"></a>אודות זהות Yammer

מומלץ שכל הרשתות י בצעו את השלבים הבאים כדי להימנע מבעיות הקשורות לזהות:

1. אכוף Office 365 זהות זו לאחר הקצאת חשבונות Microsoft 365 עבור משתמשים ב- Azure AD כדי לוודא שכל המשתמשים להיכנס באמצעות חשבון Microsoft 365 הראשי שלהם. לקבלת מידע נוסף, ראה [אכיפת זהות Office 365 עבור Yammer המשתמשים](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. איחוד רשתות Yammer מרובות. תצורות Yammer מדור קודם מאפשרות חיבור של רשתות Yammer מרובות לדייר אחד. לקבלת מידע נוסף, ראה [העברת רשת - איחוד רשתות Yammer מרובות.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. לחלופין, אכוף רישוי Yammer כדי לחסום משתמשים Yammer אם אין להם רשיון. לקבלת מידע נוסף, ראה [ניהול Yammer משתמשים ב- Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. לבסוף, בצע ביקורת על רשימת המשתמשים עבור רשתות Yammer ישנות יותר והשעה משתמשים מדור קודם. מומלץ להשעות (לבטל את ההפעלה) של משתמשים במקום למחוק אותם, מכיוון ש המחיקה אינה הפיכה. לקבלת מידע נוסף, [ראה ביקורת Yammer משתמשים ברשתות המחוברות ל- Office 365 והסרה](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) של [משתמשים](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

על-ידי קביעת Yammer באמצעות שלבים אלה, תהיה מוכן גם לקבוע את תצורת Yammer עבור מצב מקורי עבור Microsoft 365. לקבלת מידע נוסף, ראה [קביעת תצורה Yammer עבור מצב מקורי עבור Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).