---
title: Access נדחתה בעת הצגת זרימת עבודה
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495824"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="93cb4-102">Access נדחתה בעת הצגת זרימת עבודה</span><span class="sxs-lookup"><span data-stu-id="93cb4-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="93cb4-103">זרימות עבודה 2013 SharePoint המנסות לשלוח דואר אלקטרוני אל קבוצת SharePoint עלולים להיכשל עם הודעת שגיאה "Access נדחתה" אם החברות בקבוצת SharePoint אינו מוגדר לכולם.</span><span class="sxs-lookup"><span data-stu-id="93cb4-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="93cb4-104">**כדי לפתור בעיה זו, בצע את הפעולות הבאות:**</span><span class="sxs-lookup"><span data-stu-id="93cb4-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="93cb4-105">אפשר את כולם לראות את חברי קבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="93cb4-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="93cb4-106">הסר את הקבוצה SharePoint אל או עותק שורה של הודעת הדואר האלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="93cb4-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="93cb4-107">להוסיף באופן מפורש את המשתמשים אל או עותק שורה אם לא ניתן לשנות את הניראות של חברות עבור קבוצת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="93cb4-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="93cb4-108">כדי להציג פרטים נוספים נא עיין [בלתי מורשית של HTTP כדי /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="93cb4-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  