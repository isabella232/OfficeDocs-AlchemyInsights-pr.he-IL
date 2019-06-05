---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719518"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint או OneDrive איטי, נגיש או אינו זמין עבור משתמשים מרובים

אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שקיימת בעיית שירות זמניים. [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>רשיון המשתמש ולהוסיף

ודא שאתה [מקצה רשיונות המשתמשים ב- Office 365 עבור העסק](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>הקצאת הרשאות

אם למשתמש זה הוקצה רשיון Sharepoint והוא עדיין מקבל הודעה שהגישה נדחתה, נא ודא שלהם את [רמת ההרשאה המתאימה](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) שהוקצתה.

## <a name="consider-using-the-access-request-feature"></a>עליך לשקול את השימוש בתכונה בקשת גישה

[התכונה בקשת גישה](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) מאפשר לאנשים לבקש גישה לתוכן אין כעת להם הרשאה לראות.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>אפשר בקובץ script מותאם אישית עלול לגרום בעיות גישה

ישנם תרחישים מסוימים כאשר התכונה *אפשר בקובץ script מותאם אישית* עשוי להיות הצגת שהגישה נדחתה. לקבלת רשימה של תכונות המושפעות, שיקולי אבטחה ואת היכולת להשבית את התכונה. נא בקר ב- [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

