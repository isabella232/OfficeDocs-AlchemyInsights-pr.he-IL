---
title: הערות על פריטי רשימה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982492"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="a4bb4-102">הערות על פריטי רשימה</span><span class="sxs-lookup"><span data-stu-id="a4bb4-102">Comments on List items</span></span>

<span data-ttu-id="a4bb4-103">בקרוב משתמשים יוכלו להוסיף ולמחוק הערות בפריטי רשימה.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="a4bb4-104">המשתמשים יכולים להציג את כל ההערות בפריט רשימה ולסנן בין תצוגות המציגות הערות או פעילות הקשורות לפריט.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="a4bb4-105">**תזמון** :</span><span class="sxs-lookup"><span data-stu-id="a4bb4-105">**Timing** :</span></span>

<span data-ttu-id="a4bb4-106">**מהדורה ממוקדת** : הדרגתי נפתחת באמצע אוקטובר וצפויה להתבצע עד אמצע נובמבר</span><span class="sxs-lookup"><span data-stu-id="a4bb4-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="a4bb4-107">**מהדורה רגילה** : הדרגתי נפתחת באמצע נובמבר וצפויה להתבצע עד לתחילת דצמבר</span><span class="sxs-lookup"><span data-stu-id="a4bb4-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="a4bb4-108">**פריסה** : הפצה ייעודית עבור הארגון כולו</span><span class="sxs-lookup"><span data-stu-id="a4bb4-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="a4bb4-109">המשתמשים צריכים לציין את הפרטים הבאים לפני שיוכלו להוסיף ולמחוק הערות:</span><span class="sxs-lookup"><span data-stu-id="a4bb4-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="a4bb4-110">הערות מתבצעות בהתאם להגדרות ההרשאות הטבועות ב-SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="a4bb4-111">רשימות קלאסיות שעדיין אינן מוכללות להצגה בממשקי משתמש מודרני, כגון רשימות משימות, לא תכלול תכונה זו של הערות.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="a4bb4-112">הוספת הערות לרשימות ב-Teams אינה זמינה במהדורה זו.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="a4bb4-113">הערות אינן נכללות באינדקס על-ידי חיפוש.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="a4bb4-114">מנהלי מערכת יכולים להפוך תכונה זו ללא זמינה ברמת הארגון על-ידי שינוי הפרמטר **CommentsOnListItemsDisabled** ב-cmdlet **Set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="a4bb4-115">לא ניתן כעת להפוך הערות ללא זמינות באתר או ברמת הרשימה.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="a4bb4-116">אנו מקווים שפקדים אלה ייכנסו לעדכון מאוחר יותר, סביר להניח שברבעון 2021 הראשון.</span><span class="sxs-lookup"><span data-stu-id="a4bb4-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
