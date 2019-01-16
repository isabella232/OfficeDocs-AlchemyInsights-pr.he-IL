---
title: אין אפשרות להוסיף זרימת עבודה של אישור 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292964"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="cee08-102">אין אפשרות להוסיף זרימת עבודה של אישור 2010</span><span class="sxs-lookup"><span data-stu-id="cee08-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="cee08-103">באוסף אתרים של Microsoft SharePoint, אין באפשרותך להוסיף זרימת עבודה הניתנת לשימוש חוזר כללי (כגון "אישור - SharePoint 2010") רשימה או ספריה.</span><span class="sxs-lookup"><span data-stu-id="cee08-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="cee08-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="cee08-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="cee08-105">פתח את אתר הבסיס של אוסף האתרים ב- SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="cee08-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="cee08-106">תחת **אובייקטים של אתר**, בחר **זרימות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="cee08-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="cee08-107">במקטע **חדש** של רצועת הכלים של **זרימות עבודה** , בחר את **זרימת העבודה הניתן לשימוש חוזר**.</span><span class="sxs-lookup"><span data-stu-id="cee08-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="cee08-p101">בטופס ' **צור זרימת עבודה הניתן לשימוש חוזר** ', הזן את השם \* \* *Repair2010* \* \*. עבור **סוג פלטפורמה**, לחץ על **זרימת עבודה של SharePoint 2010**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="cee08-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="cee08-110">במקטע **שמירה** של רצועת הכלים של **זרימת עבודה** , בחר **פרסום**.</span><span class="sxs-lookup"><span data-stu-id="cee08-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="cee08-p102">במקטע **ניהול** של רצועת הכלים של **זרימת עבודה** , בחר **לפרסם באופן כללי**. בתיבת הדו-שיח אישור המופיעה, לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="cee08-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="cee08-p103">בדפדפן אינטרנט, אתר את אתר הבסיס של אוסף האתרים ולאחר מכן לגשת **הגדרות האתר** \> **תכונות אוסף אתרים**. להחליף את התכונה **זרימות עבודה** :</span><span class="sxs-lookup"><span data-stu-id="cee08-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="cee08-115">· אם התכונה היא *הופעל* , לחץ על **בטל הפעלה,** ולאחר מכן לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="cee08-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="cee08-116">· אם התכונה היא *Deactivated* , לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="cee08-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="cee08-117">לקבלת מידע נוסף, עיין [במאמר](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)הבא.</span><span class="sxs-lookup"><span data-stu-id="cee08-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

