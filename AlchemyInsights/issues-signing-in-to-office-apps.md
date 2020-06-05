---
title: בעיות בכניסה לאפליקציות של Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579938"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>תיקון האפליקציות של Microsoft 365 "מצטערים, חשבון נוסף מהארגון שלך כבר נחתם בהודעה"

כדי לתקן שגיאה זו, נסה את השלבים הבאים:

- הסר את כל חשבונות העבודה, למעט החשבון המושפע, באמצעות הגדרות Windows _ **הגישה לעבודה או לבית הספר**.
- [נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0. (לשעבר: \Software\Microsoft\Office\16.0\Common\Identity\)
- פתח יישום Office, בחר באפשרות ' צא **File**  >  **מחשבון**קובץ '  >  **Sign Out**. לאחר מכן, היכנס באמצעות חשבון משתמש עם רשיון חוקי. לקבלת מידע, ראה [חשבונות ב- Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- עבור Mac, ראה [לא ניתן להיכנס לאפליקציית Office 2016 עבור Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

לקבלת מידע נוסף, ראה ["מצטערים, חשבון נוסף מהארגון שלך כבר מחובר למחשב זה" ב-Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).