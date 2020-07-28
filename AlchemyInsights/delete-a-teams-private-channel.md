---
title: מחיקת ערוץ פרטי של צוותים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439327"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="ff3dc-102">מחיקת ערוץ פרטי של צוותים</span><span class="sxs-lookup"><span data-stu-id="ff3dc-102">Delete a Teams private channel</span></span>

<span data-ttu-id="ff3dc-103">מיקרוסופט מודעת לבעיה שתמחק ערוץ פרטי של צוותים אם יש לך מדיניות שמירה של SharePoint זמינה עבור אתר SharePoint המשמש כבסיס.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="ff3dc-104">מיקרוסופט עובדת על תיקון.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="ff3dc-105">בינתיים, באפשרותך להשתמש בדרכים הבאות לעקיפת השימוש כדי למחוק את הערוץ הפרטי.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="ff3dc-106">**אל תכלול את אוסף הצוות/אתר ממדיניות השמירה של Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="ff3dc-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="ff3dc-107">עבור אל פורטל הניהול של Office 365, ובחר **הצג הכל** בחלונית הניווט השמאלית.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="ff3dc-108">תחת **מרכזי ניהול**, עבור אל **אבטחה _ אמפר _**  >  מדיניות תאימות**למניעת אובדן נתונים**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="ff3dc-109">זהה כל מדיניות החלה על אתרי Sharepoint ושנה את המדיניות כך שאתר Sharepoint עבור הצוות המכיל את הערוץ הפרטי אינו נכלל תחת מדיניות השמירה.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="ff3dc-110">שמור את המדיניות.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-110">Save the policy.</span></span>
    <span data-ttu-id="ff3dc-111">זה יכול להימשך עד 24 שעות כדי שהגדרות המדיניות ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="ff3dc-112">לאחר שהאתר לא נכלל, באפשרותך למחוק את הערוץ הפרטי.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="ff3dc-113">***ייתכן*** שתוכל למחוק את הערוץ הפרטי באמצעות צוותי Microsoft בהתקן Android.</span><span class="sxs-lookup"><span data-stu-id="ff3dc-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="ff3dc-114">לקבלת מידע אודות SharePoint קשור, ראה [אין אפשרות למחוק פריטים ב-SharePoint Online או OneDrive עבור Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="ff3dc-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>