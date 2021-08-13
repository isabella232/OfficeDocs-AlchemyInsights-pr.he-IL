---
title: בעיות ביצועים- SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093735"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint או OneDrive איטי, לא נגיש או לא זמין עבור משתמשים מרובים

אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהייתה להם גישה בעבר, ייתכן שיש בעיית שירות זמנית. [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).

**הוספה ורשיון של המשתמש**

ודא שאתה [מקצה רשיונות למשתמשים Microsoft 365 לעסקים](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**הקצאת הרשאות**

אם למשתמש הוקצה רשיון Sharepoint ועדיין מקבל הודעה נדחתה על גישה, ודא שרמת ההרשאה [המתאימה הוקצתה](https://docs.microsoft.com/sharepoint/understanding-permission-levels) לו.

**שקול להשתמש בתכונת בקשת הגישה**

תכונת [בקשת הגישה](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) מאפשרת לאנשים לבקש גישה לתוכן שהם אינם כוללים כעת הרשאה לראות.

**אפשר קובץ Script מותאם אישית עלול לגרום לבעיות בגישה שנדחתה**

קיימים תרחישים מסוימים *כוללים את התכונה אפשר קובץ Script* מותאם אישית עשויה להציג גישה נדחתה. לקבלת רשימה של תכונות המושפעות, שיקולי אבטחה והיכולת להפוך את התכונה ללא זמינה. בקר [ב- אפשר או מנע קובץ Script מותאם אישית.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

