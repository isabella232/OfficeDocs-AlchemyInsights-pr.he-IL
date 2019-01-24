---
title: Access נדחתה בעת הצגת זרימת עבודה
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472338"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="87433-102">Access נדחתה בעת הצגת זרימת עבודה</span><span class="sxs-lookup"><span data-stu-id="87433-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="87433-103">זרימות עבודה 2013 SharePoint המנסות לשלוח דואר אלקטרוני אל קבוצת SharePoint עלולים להיכשל עם הודעת שגיאה "Access נדחתה" אם החברות בקבוצת SharePoint אינו מוגדר לכולם.</span><span class="sxs-lookup"><span data-stu-id="87433-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="87433-104">**כדי לפתור בעיה זו, בצע את הפעולות הבאות:**</span><span class="sxs-lookup"><span data-stu-id="87433-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="87433-105">אפשר את כולם לראות את חברי קבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="87433-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="87433-106">הסר את הקבוצה SharePoint אל או עותק שורה של הודעת הדואר האלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="87433-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="87433-107">להוסיף באופן מפורש את המשתמשים אל או עותק שורה אם לא ניתן לשנות את הניראות של חברות עבור קבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="87433-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="87433-108">כדי להציג פרטים נוספים נא עיין [בלתי מורשית של HTTP כדי /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="87433-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

