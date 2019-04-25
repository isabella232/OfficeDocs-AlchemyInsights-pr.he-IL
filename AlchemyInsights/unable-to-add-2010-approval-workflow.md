---
title: אין אפשרות להוסיף זרימת עבודה של אישור 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366836"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="0ce3e-102">אין אפשרות להוסיף זרימת עבודה של אישור 2010</span><span class="sxs-lookup"><span data-stu-id="0ce3e-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="0ce3e-103">באוסף אתרים של Microsoft SharePoint, אין באפשרותך להוסיף זרימת עבודה הניתנת לשימוש חוזר כללי (כגון "אישור - SharePoint 2010") רשימה או ספריה.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0ce3e-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0ce3e-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0ce3e-105">פתח את אתר הבסיס של אוסף האתרים ב- SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0ce3e-106">תחת **אובייקטים של אתר**, בחר **זרימות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0ce3e-107">במקטע **חדש** של רצועת הכלים של **זרימות עבודה** , בחר את **זרימת העבודה הניתן לשימוש חוזר**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0ce3e-108">בטופס ' **צור זרימת עבודה הניתן לשימוש חוזר** ', הזן את השם \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0ce3e-109">עבור **סוג פלטפורמה**, לחץ על **זרימת עבודה של SharePoint 2010**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0ce3e-110">במקטע **שמירה** של רצועת הכלים של **זרימת עבודה** , בחר **פרסום**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0ce3e-111">במקטע **ניהול** של רצועת הכלים של **זרימת עבודה** , בחר **לפרסם באופן כללי**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0ce3e-112">בתיבת הדו-שיח אישור המופיעה, לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0ce3e-113">בדפדפן אינטרנט, אתר את אתר הבסיס של אוסף האתרים ולאחר מכן לגשת **הגדרות האתר** \> **תכונות אוסף אתרים**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0ce3e-114">להחליף את התכונה **זרימות עבודה** :</span><span class="sxs-lookup"><span data-stu-id="0ce3e-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0ce3e-115">· אם התכונה היא *הופעל* , לחץ על **בטל הפעלה,** ולאחר מכן לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0ce3e-116">· אם התכונה היא *Deactivated* , לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0ce3e-117">לקבלת מידע נוסף, עיין [במאמר](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)הבא.</span><span class="sxs-lookup"><span data-stu-id="0ce3e-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

