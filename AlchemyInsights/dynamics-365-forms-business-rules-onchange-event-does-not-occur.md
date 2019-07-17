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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="59a05-102">אירוע OnChange אינה מתרחשת אם השדה משתנה באופן תוכניתי</span><span class="sxs-lookup"><span data-stu-id="59a05-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="59a05-103">האירוע *OnChange* מתרחש אם השדה משתנה באופן תוכניתי באמצעות ה *התכונה.* שיטת [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="59a05-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="59a05-104">אם ברצונך מטפלים באירועים עבור אירוע *OnChange* לפעול לאחר שהגדרת את ערך עליך להשתמש *התכונה formContext.data.entity.* שיטת [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) בקוד שלך.</span><span class="sxs-lookup"><span data-stu-id="59a05-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
