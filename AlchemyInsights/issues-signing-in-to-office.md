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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579902"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>מסך כניסה ריק ב-Microsoft 365 אפליקציות

כדי לפתור בעיה זו, נסה את הפעולות הבאות:
- התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- איפוס אפשרויות internet explorer: עבור אל **כלים**  >  **אפשרויות אינטרנט**  >  איפוס**מתקדם**  >  **של הגדרות internet explorer** (שים לב שתאבד הגדרות מותאמות אישית) ולאחר מכן נסה שוב להיכנס ל-Office.
- בטל את משמר היישומים של Windows Defender (WDAG) או כל חומת אש או תוכנית אנטי-וירוס דומה:
    1. בלוח הבקרה, עבור אל **תוכניות**ולאחר מכן בחר **באפשרות הפעל או בטל את התכונות של Windows**.
    2. אם Windows Defender משמר היישומים מופעל, נסה להשבית אותו.<br/>
    **הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.
- ודא שיישום [plug-In](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) של Microsoft. BROKERPLUGIN עמ מ של מיקרוסופט אינו נחסם על-ידי יישומים או חומת אש/תוכנת אנטי-וירוס כלשהם.
- [נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0. (לשעבר: \Software\Microsoft\Office\16.0\Common\Identity\)

לקבלת מידע נוסף, ראה [בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 build 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).