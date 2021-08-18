---
title: בעיות בכניסה לאפליקציות Microsoft 365 שלך
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088037"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>מסך כניסה ריק באפליקציות Microsoft 365 בלבד

כדי לפתור בעיה זו, נסה את הפעולות הבאות:
- התקן את העדכונים האחרונים [עבור Windows ו-](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- איפוס אפשרויות Internet Explorer: עבור **אל** כלים אפשרויות אינטרנט איפוס מתקדם של Internet Explorer הגדרות (שים לב שתאבד הגדרות מותאמות אישית) ולאחר מכן נסה שוב  >    >    >   להיכנס ל- Office.
- הפוך את Windows Defender Application Guard (WDAG) ללא זמין או כל תוכנית דומה של חומת אש או אנטי-וירוס:
    1. בלוח הבקרה, עבור אל **תוכניות** ולאחר מכן בחר **הפעל או בטל Windows תכונות בקרה.**
    2. אם Windows Defender Application Guard זמינה, נסה להפוך אותה ללא זמינה.<br/>
    **הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.
- ודא ש- Plug-in של Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) אינו נחסם על-ידי יישום או חומת אש/תוכנית אנטי-וירוס.
- [נקה Office אישורי](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows מנהל האישורים.<br/>
    **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל- 16.0. (לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)

לקבלת מידע נוסף, ראה בעיות חיבור בהתחברות לאחר עדכון [ל- Office גירסת Build מס' 16.0.7967 ב- Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)