---
title: כללים עסקיים של Dynamics 365 Forms - כלל עסקי לא יורים עבור טופס
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
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947300"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>האירוע OnChange אינו מתרחש אם השדה משתנה באופן תיכנותי

האירוע *OnChange* אינו מתרחש אם השדה משתנה באופן תיכנותי באמצעות *התכונה.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method. אם ברצונך שמפעילי אירועים עבור *האירוע OnChange* יתנהלו לאחר הגדרת הערך, עליך להשתמש בשיטה *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) בקוד שלך.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
