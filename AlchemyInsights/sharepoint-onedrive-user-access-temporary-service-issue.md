---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771245"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint או OneDrive איטיים, לא נגישים או שאינם זמינים עבור משתמשים מרובים

אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיו ברשותם גישה בעבר, ייתכן שקיימת בעיה של שירות זמני. [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).

**הוספה ורשיון של המשתמש**

ודא [שתקצה רשיונות למשתמשים ב-Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**הקצאת הרשאות**

אם למשתמש הוקצה רשיון של Sharepoint והוא עדיין מקבל הודעת גישה שנדחתה, ודא שהוקצה לה [רמת הרשאה מתאימה](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**שקול להשתמש בתכונה ' בקשת גישה '**

[התכונה ' בקשת גישה](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ' מאפשרת לאנשים לבקש גישה לתוכן שאינו כולל כעת הרשאה לראות.

**אפשר סקריפט מותאם אישית עלול לגרום לבעיות של access שנדחו**

קיימים תרחישים מסוימים שבהם ייתכן שהתכונה ' *אפשר סקריפט מותאם אישית* ' מציגה גישה שנדחתה. לקבלת רשימה של תכונות מושפעות, שיקולי אבטחה ויכולת להפוך את התכונה ללא זמינה. בקר [באפשרות אפשר או מנע סקריפט מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

