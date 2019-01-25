---
title: אין אפשרות להוסיף ברירת המחדל זרימת עבודה של אישור 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471909"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="692cb-102">אין אפשרות להוסיף ברירת המחדל זרימת עבודה של אישור 2010</span><span class="sxs-lookup"><span data-stu-id="692cb-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="692cb-103">באוסף אתרים של Microsoft SharePoint, אין באפשרותך להוסיף זרימת עבודה הניתנת לשימוש חוזר כללי (כגון "אישור - SharePoint 2010") רשימה או ספריה.</span><span class="sxs-lookup"><span data-stu-id="692cb-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="692cb-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="692cb-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="692cb-105">פתח את אתר הבסיס של אוסף האתרים ב- SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="692cb-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="692cb-106">תחת **אובייקטים של אתר**, בחר **זרימות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="692cb-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="692cb-107">במקטע **חדש** של רצועת הכלים של **זרימות עבודה** , בחר את **זרימת העבודה הניתן לשימוש חוזר**.</span><span class="sxs-lookup"><span data-stu-id="692cb-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="692cb-p101">בטופס ' **צור זרימת עבודה הניתן לשימוש חוזר** ', הזן את השם \* \*\*Repair2010\*\*\*. עבור **סוג פלטפורמה**, בחר את **זרימת העבודה של SharePoint 2010**ולאחר מכן בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="692cb-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="692cb-110">במקטע **שמירה** של רצועת הכלים של **זרימת עבודה** , בחר **פרסום**.</span><span class="sxs-lookup"><span data-stu-id="692cb-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="692cb-p102">במקטע **ניהול** של רצועת הכלים של **זרימת עבודה** , בחר **לפרסם באופן כללי**. בתיבת הדו-שיח אישור המופיעה, לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="692cb-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="692cb-p103">בדפדפן אינטרנט, אתר את אתר הבסיס של אוסף האתרים ולאחר מכן לגשת **הגדרות האתר** \> **תכונות אוסף אתרים**. לאחר מכן, להחליף את התכונה **זרימות עבודה** :</span><span class="sxs-lookup"><span data-stu-id="692cb-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="692cb-115">· אם התכונה היא *הופעל* , לחץ על **בטל הפעלה,** ולאחר מכן לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="692cb-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="692cb-116">· אם התכונה היא *Deactivated* , לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="692cb-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="692cb-117">לקבלת מידע נוסף, עיין [במאמר](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)הבא.</span><span class="sxs-lookup"><span data-stu-id="692cb-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

