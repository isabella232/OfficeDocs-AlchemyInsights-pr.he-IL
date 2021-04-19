---
title: הסתרה או ביטול הסתרה של קבוצות או צוותים של Office 365 מרשימת כתובות
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811457"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>הסתרה או ביטול הסתרה של קבוצות או צוותים של Office 365 מרשימת כתובות

השתמש בפקודה הבאה של EXO PowerShell כדי להסתיר או לבטל הסתרה של קבוצת Office 365/teams מרשימות כתובות (GAL) של לקוחות Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

השתמש בפקודה הבאה של EXO PowerShell כדי להסתיר או לבטל את הסתרת הקבוצה/הצוותים של Office365 מלקוחות Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- לקבלת הוראות מפורטות, ראה [הסתרת קבוצות Office 365 מלקוחות GAL ו- Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
