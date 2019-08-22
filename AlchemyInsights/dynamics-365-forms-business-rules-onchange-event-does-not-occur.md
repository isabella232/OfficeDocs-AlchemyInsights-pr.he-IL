---
title: Dynamics 365 טפסים כללים עסקיים - כלל עסקי לא הפעלת עבור טופס
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529020"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>אירוע OnChange אינה מתרחשת אם השדה משתנה באופן תוכניתי

האירוע *OnChange* מתרחש אם השדה משתנה באופן תוכניתי באמצעות ה *התכונה.* שיטת [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . אם ברצונך מטפלים באירועים עבור אירוע *OnChange* לפעול לאחר שהגדרת את ערך עליך להשתמש *התכונה formContext.data.entity.* שיטת [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) בקוד שלך.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
