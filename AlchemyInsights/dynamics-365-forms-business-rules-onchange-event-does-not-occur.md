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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529020"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="89c7b-102">האירוע OnChange אינו מתרחש אם השדה משתנה באופן תיכנותי</span><span class="sxs-lookup"><span data-stu-id="89c7b-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="89c7b-103">האירוע *Onchange* אינו מתרחש אם השדה משתנה באופן תיכנותי באמצעות *התכונה.* שיטת [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="89c7b-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="89c7b-104">אם ברצונך שמטפלים באירועים עבור האירוע *Onchange* יפעלו לאחר הגדרת הערך, עליך להשתמש *בתכונה formcontext. data. הישות.* שיטת [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) בקוד שלך.</span><span class="sxs-lookup"><span data-stu-id="89c7b-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
