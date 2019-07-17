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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747783"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>אירוע OnChange אינה מתרחשת אם השדה משתנה באופן תוכניתי

האירוע *OnChange* מתרחש אם השדה משתנה באופן תוכניתי באמצעות ה *התכונה.* שיטת [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . אם ברצונך מטפלים באירועים עבור אירוע *OnChange* לפעול לאחר שהגדרת את ערך עליך להשתמש *התכונה formContext.data.entity.* שיטת [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) בקוד שלך.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
