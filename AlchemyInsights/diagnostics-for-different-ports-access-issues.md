---
title: אבחון בעיות גישה ליציאות שונות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035783"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="2765d-102">אבחון בעיות גישה ליציאות שונות</span><span class="sxs-lookup"><span data-stu-id="2765d-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="2765d-103">כדי לפתור את בעיות הגישה ליציאות השונות, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2765d-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="2765d-104">עצור/בטל את ההקצאה של המחשב הווירטואלי (VM) מתוך הפורטל, הפעל מחדש את ה-VM ובדוק שוב.</span><span class="sxs-lookup"><span data-stu-id="2765d-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="2765d-105">בדוק את הגדרות הרשת של ה-VM שלך כדי לקבוע אם אתה מבצע חסימת תעבורה בקבוצות אבטחה של רשת (NSGs).</span><span class="sxs-lookup"><span data-stu-id="2765d-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="2765d-106">באפשרותך גם להשתמש [בכלי אימות זרימת הזרימה של ה-IP של הצופה ברשת](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) כדי לבדוק אם קיימות תעבורה לחסימת NSGs, מסלולי User-Defined (UDRs) ניתוב מחדש של התעבורה בחזרה למכשיר המקומי (' נתיב ברירת המחדל ' ב-0.0.0.0/0) או במכשיר רשת.</span><span class="sxs-lookup"><span data-stu-id="2765d-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="2765d-107">אם אתה עדיין נתקל בבעיות לאחר שניסית את השלבים לעיל, ספק את שם ה-VM ואת יציאת ה-TCP שאתה מנסה לשלוח בדואר לצורך אבחון נוסף.</span><span class="sxs-lookup"><span data-stu-id="2765d-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="2765d-108">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="2765d-108">**Recommended Documents**</span></span>

[<span data-ttu-id="2765d-109">מגבלות והמלצות לשליחת דואר אלקטרוני יוצא דרך יציאה 25</span><span class="sxs-lookup"><span data-stu-id="2765d-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)