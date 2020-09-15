---
title: בעיות בכניסה ליישומי Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695324"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>תיקון יישומי Microsoft 365 "מצטערים, חשבון אחר מהארגון שלך כבר מחובר ל-" message

כדי לתקן שגיאה זו, נסה את השלבים הבאים:

- הסר את כל חשבונות העבודה, למעט החשבון המושפע, באמצעות הגדרות Windows > **Access בעבודה או בבית הספר**.
- [נקה את אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום של Office 2016 השתנו ל-16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- פתח יישום של Office, בחר **File**באפשרות יציאה  >  **מחשבון**קובץ  >  **Sign Out**. לאחר מכן, היכנס באמצעות חשבון משתמש עם רשיון חוקי. לקבלת מידע, ראה [חשבונות ב- Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- עבור Mac, ראה [לא ניתן להיכנס לאפליקציית Office 2016 עבור Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

לקבלת מידע נוסף, ראה ["מצטערים, חשבון אחר מהארגון שלך כבר מחובר במחשב זה" ב-Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).