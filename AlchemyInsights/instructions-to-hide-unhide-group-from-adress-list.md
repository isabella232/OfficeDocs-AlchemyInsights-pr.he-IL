---
title: הוראות להסתיר/לבטל הסתרה של קבוצה מרשימת כתובות
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
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926246"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>הסתרת Microsoft 365 מרשימת כתובות (GAL)

כדי להסתיר קבוצת Microsoft 365 מרשימות כתובות (GAL) של לקוחות Exchange (כגון Outlook או OWA), השתמש בפקודה הבאה במעטפת EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

כדי להסתיר את Microsoft 365 כדי להיות גלויה ללקוחות Exchange, השתמש בפקודה הבאה במעטפת EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

