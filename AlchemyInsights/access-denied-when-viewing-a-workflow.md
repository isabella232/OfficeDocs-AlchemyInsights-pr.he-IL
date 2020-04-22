---
title: הגישה נדחתה בעת הצגת זרימת עבודה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687331"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="aaca5-102">הגישה נדחתה בעת הצגת זרימת עבודה</span><span class="sxs-lookup"><span data-stu-id="aaca5-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="aaca5-103">SharePoint 2013 זרימות עבודה שמנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint יכולה להיכשל בהודעת שגיאה "הגישה נדחתה" אם החברות בקבוצת SharePoint אינה מוגדרת ככולם.</span><span class="sxs-lookup"><span data-stu-id="aaca5-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="aaca5-104">**כדי לפתור בעיה זו, בצע את הפעולות הבאות:**</span><span class="sxs-lookup"><span data-stu-id="aaca5-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="aaca5-105">אפשר לכולם לראות את החברים בקבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="aaca5-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="aaca5-106">הסר את קבוצת SharePoint מהשורה ' אל ' או ' עותק ' של הדואר האלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="aaca5-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="aaca5-107">הוסף במפורש את המשתמשים לשורה ' אל ' או ' עותק ' אם אין אפשרות לשנות את ניראות החברות עבור קבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="aaca5-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="aaca5-108">כדי לצפות בפרטים נוספים, עיין ב- [HTTP לא מורשה ל/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="aaca5-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  