---
title: הוראות להסתרה/ביטול הסתרה של קבוצה מרשימת כתובות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663010"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>הסתרת קבוצת Microsoft 365 מרשימת הכתובות (GAL)

כדי להסתיר קבוצה של Microsoft 365 מרשימות כתובות (GAL) של לקוחות Exchange (כגון Outlook או OWA), השתמש בפקודה הבאה ב-קליפת shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

כדי להסתיר את הקבוצה Microsoft 365 מלהיות גלוי ללקוחות Exchange, השתמש בפקודה הבאה ב-קליפת shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

