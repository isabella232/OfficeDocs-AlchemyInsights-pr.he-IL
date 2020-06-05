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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580010"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>הסתר את קבוצת Microsoft 365 מרשימת הכתובות (GAL)

כדי להסתיר קבוצת Microsoft 365 מרשימות כתובות (GAL) של לקוחות Exchange (כגון Outlook או OWA), השתמש בפקודה הבאה במעטפת EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

כדי להסתיר את קבוצת Microsoft 365 מלהיות גלויה ללקוחות Exchange, השתמש בפקודה הבאה במעטפת EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

