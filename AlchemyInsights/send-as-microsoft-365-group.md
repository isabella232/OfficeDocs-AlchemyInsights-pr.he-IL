---
title: הקבוצה ' שלח כ-Microsoft 365 '
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871850"
---
# <a name="send-as-microsoft-365-group"></a>הקבוצה ' שלח כ-Microsoft 365 '

באפשרותך להקצות הרשאות ' שלח כ ' כדי לאפשר למשתמשים ספציפיים לשלוח הודעות כקבוצה של Microsoft 365:  

1. התחבר אל Exchange Online PowerShell.  

2. הפעל את הפקודה הבאה:  

    Add-RecipientPermission `<GroupName>` -נאמן `<MailboxName>` -AccessRights רשאת sendas עבור

לקבלת מידע נוסף, ראה [מתן אפשרות לחברים לשלוח בשם או לשלוח בשם של קבוצה](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).