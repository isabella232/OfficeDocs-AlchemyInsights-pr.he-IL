---
title: אין אפשרות להוסיף זרימת עבודה של אישור של 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699736"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="60654-102">אין אפשרות להוסיף זרימת עבודה של אישור של 2010</span><span class="sxs-lookup"><span data-stu-id="60654-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="60654-103">באוסף אתרים של Microsoft SharePoint, אין באפשרותך להוסיף זרימת עבודה הניתנת לשימוש חוזר כללי (כגון "אישור-SharePoint 2010") לרשימה או לספריה.</span><span class="sxs-lookup"><span data-stu-id="60654-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="60654-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="60654-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="60654-105">פתח את אתר האינטרנט הבסיסי של אוסף האתרים ב-SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="60654-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="60654-106">תחת **אובייקטי אתר**, בחר **זרימות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="60654-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="60654-107">במקטע **החדש** של רצועת הכלים ' **זרימות עבודה** ', בחר **זרימת עבודה הניתנת לשימוש חוזר**.</span><span class="sxs-lookup"><span data-stu-id="60654-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="60654-108">בטופס **יצירת זרימת עבודה הניתנת לשימוש חוזר** , הזן את השם \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="60654-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="60654-109">עבור **סוג פלטפורמה**, לחץ על **זרימת העבודה של SharePoint 2010**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="60654-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="60654-110">במקטע **Save** של רצועת הכלים של **זרימת העבודה** , בחר **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="60654-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="60654-111">במקטע **ניהול** של רצועת הכלים של **זרימת העבודה** , בחר פרסם באופן **כללי**.</span><span class="sxs-lookup"><span data-stu-id="60654-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="60654-112">בתיבת הדו לאישור שמופיעה, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="60654-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="60654-113">בדפדפן אינטרנט, אתר את אתר האינטרנט הבסיסי של אוסף האתרים ולאחר מכן גש **Site Settings** \> **לתכונות אוסף האתרים**של הגדרות האתר.</span><span class="sxs-lookup"><span data-stu-id="60654-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="60654-114">החלף מצב של התכונה ' **זרימות עבודה** ':</span><span class="sxs-lookup"><span data-stu-id="60654-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="60654-115">· אם התכונה  *מופעלת*  , לחץ על **בטל הפעלה** ולאחר מכן לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="60654-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="60654-116">· אם התכונה  *מבוטלת*  , לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="60654-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="60654-117">לקבלת מידע נוסף, עיין [במאמר](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)הבא.</span><span class="sxs-lookup"><span data-stu-id="60654-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

