---
title: הוראות להסתרה/בהסתרה של קבוצה מרשימת כתובות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908345"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>הסתר את קבוצת Microsoft 365 מרשימת הכתובות (GAL)

כדי להסתיר קבוצת Microsoft 365 מרשימות כתובות (GAL) של לקוחות Exchange (כגון Outlook או OWA), השתמש בפקודה הבאה במעטפת EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

כדי להסתיר את קבוצת Microsoft 365 מלהיות גלויה ללקוחות Exchange, השתמש בפקודה הבאה במעטפת EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

