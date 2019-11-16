---
title: Dynamics 365 כללי עסקים-כלל עסקי לא יורים לטופס
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769340"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>האירוע OnChange אינו מתרחש אם השדה משתנה באופן תיכנותי

האירוע *Onchange* אינו מתרחש אם השדה משתנה באופן תיכנותי באמצעות *התכונה.* שיטת [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . אם ברצונך שמטפלים באירועים עבור האירוע *Onchange* יפעלו לאחר הגדרת הערך, עליך להשתמש [בפעולת](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) השירות *formcontext. data. הישות* בקוד שלך.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
