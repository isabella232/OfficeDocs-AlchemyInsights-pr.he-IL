---
title: הפעלת זרימת עבודה חסרה נכשלה
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36753797"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="1f4ad-102">הפעלת זרימת עבודה חסרה נכשלה</span><span class="sxs-lookup"><span data-stu-id="1f4ad-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="1f4ad-103">באוסף אתרים של Microsoft SharePoint, אין באפשרותך להוסיף זרימת עבודה גלובלית הניתנת לשימוש חוזר (כגון "אישור-SharePoint 2010") לרשימה או ספריה.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="1f4ad-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1f4ad-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="1f4ad-105">פתח את אתר השורש של אוסף האתרים ב-SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="1f4ad-106">תחת **אובייקטי אתר**, בחר **זרימות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="1f4ad-107">במקטע **החדש** של רצועת הכלים **זרימות עבודה** , בחר באפשרות **זרימת עבודה הניתנת לשימוש חוזר**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="1f4ad-108">בטופס **יצירת זרימת עבודה לשימוש חוזר** , הזן את השם \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="1f4ad-109">עבור **סוג פלטפורמה**, לחץ על **SharePoint 2010 זרימת עבודה**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="1f4ad-110">במקטע **Save** ברצועת הכלים **זרימת עבודה** , בחר **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="1f4ad-111">במקטע **ניהול** של רצועת הכלים **זרימת עבודה** , בחר פרסם באופן **גלובלי**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="1f4ad-112">בתיבת הדו של האישור שמופיעה, בחר **ב'אישור '**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="1f4ad-113">בדפדפן אינטרנט, אתר את אתר הבסיס של אוסף האתרים ולאחר מכן גש \> **לתכונות אוסף אתרים**של **הגדרות אתר** .</span><span class="sxs-lookup"><span data-stu-id="1f4ad-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="1f4ad-114">לאחר מכן, החלף את התכונה ' **זרימות עבודה** ':</span><span class="sxs-lookup"><span data-stu-id="1f4ad-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="1f4ad-115">· אם התכונה *מופעלת* , לחץ על **בטל הפעלה** ולאחר מכן לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="1f4ad-116">· אם התכונה *מבוטלת* , לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="1f4ad-117">לקבלת מידע נוסף, עיין [במאמר](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)הבא.</span><span class="sxs-lookup"><span data-stu-id="1f4ad-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

