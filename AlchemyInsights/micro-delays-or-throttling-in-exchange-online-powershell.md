---
title: מיקרו עיכובים או ויסות ב- Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098567"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>מיקרו עיכובים או ויסות ב- Exchange Online PowerShell

ייתכן שתראה אזהרות "מיקרו עיכוב הוחל" או עיכובים כאשר בעת הפעלת קובצי Script או cmdlets ב- Exchange Online. להלן כמה הצעות כיצד לפתור את הבעיה:

- הפעל את האבחון שלנו כדי להירגע מדיניות ויסות PowerShell של הדייר שלך. פתרון זה יפתור את הבעיה לרוב.
- אם הבעיה עדיין לא נפתרה, [השתמש במודול Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), הכולל כלי CMDlet המבוססים על REST API והם מבצעים באופן משמעותי יותר. פעולה זו עשויה להיות פתרון מצוין עבור רכיבי Get- CMDlets רבים שנמצאים בשימוש לעיתים קרובות.
- אם עליך להשתמש ברכיבי CMDlet שלא מכוסים במודול v2, ראה הפעלת [כלי cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)של PowerShell עבור מספר גדול של משתמשים ב- Office 365 , אשר מדבר על האופן שבו ניתן לעקוף את מגבלות ויסות PowerShell ב- Exchange Online.
