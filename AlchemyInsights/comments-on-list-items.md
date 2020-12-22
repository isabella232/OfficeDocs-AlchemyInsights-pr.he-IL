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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724155"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="f69fb-102">הערות על פריטי רשימה</span><span class="sxs-lookup"><span data-stu-id="f69fb-102">Comments on List items</span></span>

<span data-ttu-id="f69fb-103">המשתמשים יכולים להציג את כל ההערות בפריט רשימה ולסנן בין תצוגות המציגות הערות או פעילות הקשורות לפריט.</span><span class="sxs-lookup"><span data-stu-id="f69fb-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="f69fb-104">המשתמשים צריכים לציין את הפרטים הבאים לפני שיוכלו להוסיף ולמחוק הערות:</span><span class="sxs-lookup"><span data-stu-id="f69fb-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="f69fb-105">הערות מתבצעות בהתאם להגדרות ההרשאות הטבועות ב-SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f69fb-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="f69fb-106">רשימות קלאסיות שעדיין אינן מוכללות להצגה בממשקי משתמש מודרני, כגון רשימות משימות, לא תכלול תכונה זו של הערות.</span><span class="sxs-lookup"><span data-stu-id="f69fb-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="f69fb-107">הוספת הערות לרשימות ב-Teams אינה זמינה במהדורה זו.</span><span class="sxs-lookup"><span data-stu-id="f69fb-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="f69fb-108">הערות אינן נכללות באינדקס על-ידי חיפוש.</span><span class="sxs-lookup"><span data-stu-id="f69fb-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="f69fb-109">מנהלי מערכת יכולים להפוך תכונה זו ללא זמינה ברמת הארגון על-ידי שינוי הפרמטר **CommentsOnListItemsDisabled** ב-cmdlet **Set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f69fb-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="f69fb-110">לא ניתן כעת להפוך הערות ללא זמינות באתר או ברמת הרשימה.</span><span class="sxs-lookup"><span data-stu-id="f69fb-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="f69fb-111">אנו מקווים שפקדים אלה ייכנסו לעדכון מאוחר יותר, סביר להניח שברבעון 2021 הראשון.</span><span class="sxs-lookup"><span data-stu-id="f69fb-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
