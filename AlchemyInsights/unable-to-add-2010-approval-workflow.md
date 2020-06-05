---
title: אין אפשרות להוסיף 2010 זרימת עבודה של אישור
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582848"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="848e1-102">אין אפשרות להוסיף 2010 זרימת עבודה של אישור</span><span class="sxs-lookup"><span data-stu-id="848e1-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="848e1-103">באוסף אתרים של Microsoft SharePoint, אין באפשרותך להוסיף זרימת עבודה גלובלית הניתנת לשימוש חוזר (כגון "אישור-SharePoint 2010") לרשימה או ספריה.</span><span class="sxs-lookup"><span data-stu-id="848e1-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="848e1-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="848e1-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="848e1-105">פתח את אתר השורש של אוסף האתרים ב-SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="848e1-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="848e1-106">תחת **אובייקטי אתר**, בחר **זרימות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="848e1-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="848e1-107">במקטע **החדש** של רצועת הכלים **זרימות עבודה** , בחר באפשרות **זרימת עבודה הניתנת לשימוש חוזר**.</span><span class="sxs-lookup"><span data-stu-id="848e1-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="848e1-108">בטופס **יצירת זרימת עבודה לשימוש חוזר** , הזן את השם \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="848e1-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="848e1-109">עבור **סוג פלטפורמה**, לחץ על **SharePoint 2010 זרימת עבודה**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="848e1-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="848e1-110">במקטע **Save** ברצועת הכלים **זרימת עבודה** , בחר **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="848e1-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="848e1-111">במקטע **ניהול** של רצועת הכלים **זרימת עבודה** , בחר פרסם באופן **גלובלי**.</span><span class="sxs-lookup"><span data-stu-id="848e1-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="848e1-112">בתיבת הדו של האישור שמופיעה, בחר **ב'אישור '**.</span><span class="sxs-lookup"><span data-stu-id="848e1-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="848e1-113">בדפדפן אינטרנט, אתר את אתר הבסיס של אוסף האתרים ולאחר מכן **Site Settings** גש \> **לתכונות אוסף האתרים**של הגדרות אתר.</span><span class="sxs-lookup"><span data-stu-id="848e1-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="848e1-114">החלף את התכונה ' **זרימות עבודה** ':</span><span class="sxs-lookup"><span data-stu-id="848e1-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="848e1-115">· אם התכונה *מופעלת* , לחץ על **בטל הפעלה** ולאחר מכן לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="848e1-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="848e1-116">· אם התכונה *מבוטלת* , לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="848e1-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="848e1-117">לקבלת מידע נוסף, עיין [במאמר](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)הבא.</span><span class="sxs-lookup"><span data-stu-id="848e1-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

