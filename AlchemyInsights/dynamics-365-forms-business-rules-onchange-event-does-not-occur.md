---
title: כללי Business של Dynamics 365-כלל עסקי אינם יורים עבור טופס
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711492"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>אירוע OnChange אינו מתרחש אם השדה משתנה באופן תוכניתי

האירוע *OnChange* אינו מתרחש אם השדה משתנה באופן תוכניתי באמצעות *התכונה.* שיטת [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . אם ברצונך שמטפלים *באירועים* יופעלו לאחר הגדרת הערך, עליך להשתמש *בתכונה formContext. data.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) בקוד שלך.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
