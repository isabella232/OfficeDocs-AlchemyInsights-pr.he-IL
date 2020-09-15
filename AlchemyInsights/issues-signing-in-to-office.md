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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695288"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>מסך כניסה ריקה ביישומי Microsoft 365

כדי לפתור בעיה זו, נסה את הפעולות הבאות:
- התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- איפוס אפשרויות internet explorer: עבור אל **כלים**  >  **אפשרויות אינטרנט**  >  **מתקדמות**  >  **איפוס הגדרות internet Explorer** (שים לב שתאבד הגדרות מותאמות אישית) ולאחר מכן נסה להיכנס שוב ל-Office.
- הפוך את מרכז היישומים של Windows Defender ללא זמין (WDAG) או כל חומת אש דומה או תוכנית אנטי-וירוס דומה:
    1. בלוח הבקרה, עבור אל **תוכניות**ולאחר מכן בחר **באפשרות הפעלה או ביטול של תכונות Windows**.
    2. אם משמר היישומים של Windows Defender מופעל, נסה להפוך אותו ללא זמין.<br/>
    **הערה:** ייתכן שתצטרך להפעיל מחדש את המחשב.
- ודא [שהתוסף](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) של MICROSOFT. עמ BrokerPlugin פטיש רטוב אינו נחסם על-ידי יישום או תוכנית חומת אש/אנטי-וירוס.
- [נקה את אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום של Office 2016 השתנו ל-16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

לקבלת מידע נוסף, ראה [בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 build 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).