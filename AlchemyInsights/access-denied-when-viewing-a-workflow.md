---
title: Access נדחה בעת הצגת זרימת עבודה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688803"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="7a97f-102">Access נדחה בעת הצגת זרימת עבודה</span><span class="sxs-lookup"><span data-stu-id="7a97f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="7a97f-103">זרימות עבודה של SharePoint 2013 המנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint יכולה להיכשל עם הודעת השגיאה "הגישה נדחתה" אם החברות בקבוצת SharePoint אינה מוגדרת לכולם.</span><span class="sxs-lookup"><span data-stu-id="7a97f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="7a97f-104">**כדי לפתור בעיה זו, בצע שלבים אלה:**</span><span class="sxs-lookup"><span data-stu-id="7a97f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="7a97f-105">אפשר לכולם לראות את החברים בקבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7a97f-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="7a97f-106">הסר את הקבוצה של SharePoint מהשורה אל או עותק של הודעת הדואר האלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="7a97f-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="7a97f-107">הוסף את המשתמשים באופן מפורש לשורה ' אל ' או ' עותק ' אם לא ניתן לשנות את ניראות החברות עבור קבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7a97f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="7a97f-108">כדי להציג פרטים נוספים, עיין במאמר [HTTP לא מורשה ל/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7a97f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  