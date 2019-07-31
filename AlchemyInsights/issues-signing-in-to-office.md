---
title: בעיות הכניסה אל יישומי Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938231"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>מסך הכניסה ריק ב- Office apps

כדי לפתור בעיה זו, נסה את הפעולות הבאות:
- התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- איפוס Internet Explorer אפשרויות: עבור אל **כלי** > **אפשרויות אינטרנט** > **מתקדם** > **איפוס הגדרות Internet Explorer** (הערה תאבד את הגדרות מותאמות אישית) ולאחר מכן נסה שוב להיכנס ל- Office.
- השבת את מגן יישום של Windows Defender (WDAG) או כל תוכנית חומת אש או אנטי-וירוס דומה:
    1. בלוח הבקרה, לעבור על **תוכניות**ולאחר מכן בחר את **תכונות Windows להפעיל או לבטל**.
    2. אם מגן יישום של Windows Defender זמינה, נסה להפוך אותה ללא זמינה.<br/>
    **הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.
- ודא כי Microsoft.AAD.BrokerPlugin [WAM AAD יישום plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) אינה חסומה על-ידי כל יישום או תוכנית חומת אש/anti-virus.
- [אישורי Office ניקוי](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי רישום עבור Office 2016 השתנו כדי 16.0. (לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)

לקבלת מידע נוסף, ראה [חיבור בעיות בהכניסה לאחר העדכון ל- Office 2016 build 16.0.7967 על Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).