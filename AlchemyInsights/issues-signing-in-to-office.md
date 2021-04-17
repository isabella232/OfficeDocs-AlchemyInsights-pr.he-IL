---
title: בעיות בכניסה לאפליקציות Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833040"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>מסך כניסה ריק באפליקציות Microsoft 365

כדי לפתור בעיה זו, נסה את הפעולות הבאות:
- התקן את העדכונים האחרונים עבור [Windows ו-](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- איפוס אפשרויות Internet Explorer: עבור **אל** כלים אפשרויות אינטרנט הגדרות מתקדמות של איפוס Internet Explorer (שים לב שתאבד  >    >    >   הגדרות מותאמות אישית) ולאחר מכן נסה שוב להיכנס ל- Office.
- הפוך את Windows Defender Application Guard (WDAG) ללא זמין או כל חומת אש דומה או תוכנית אנטי-וירוס:
    1. בלוח הבקרה, עבור אל **תוכניות** ולאחר מכן בחר **הפעל או בטל תכונות Windows**.
    2. אם Windows Defender Application Guard זמין, נסה להפוך אותו ללא זמין.<br/>
    **הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.
- ודא ש- Plug-in של Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) אינו נחסם על-ידי יישום או חומת אש/תוכנית אנטי-וירוס.
- [נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל- 16.0. (לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)

לקבלת מידע נוסף, ראה בעיות חיבור בהתחברות לאחר עדכון ל- [Office 2016 גירסת Build מס' 16.0.7967 ב- Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)