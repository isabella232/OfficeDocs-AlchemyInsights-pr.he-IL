---
title: מיקרו עיכובים או ויסות ב- Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947912"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>מיקרו עיכובים או ויסות ב- Exchange Online PowerShell

ייתכן שתראה אזהרות "מיקרו עיכוב הוחל" או עיכובים כאשר בעת הפעלת קובצי Script או cmdlets ב- Exchange Online. להלן שתי הצעות הקשורות לכך:

- ייתכן שתרצה לנסות להשתמש ב[מודול Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), הכולל את רכיבי ה-CMDlet המבוססים על REST API ובעלי ביצועים טובים יותר באופן משמעותי. פעולה זו עשויה להיות פתרון מצוין עבור רכיבי Get- CMDlets רבים שנמצאים בשימוש לעיתים קרובות.
- אם עליך להשתמש ברכיבי CMDlet שאינם מכוסים עדיין במודול v2, ראה את הנושא [הפעלה באמצעות רכיבי cmdlet של PowerShell עבור מספר גדול של משתמשים ב- Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), שדן בכיצד ניתן לעקוף מגבלות ויסות צפויות של PowerShell ב- Exchange Online.
