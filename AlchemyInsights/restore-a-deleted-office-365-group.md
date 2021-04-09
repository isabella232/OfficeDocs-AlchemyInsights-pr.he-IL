---
title: שחזור קבוצה שנמחקה של Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645132"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="8fe4f-102">שחזור קבוצה שנמחקה של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8fe4f-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="8fe4f-103">באפשרותך לשחזר קבוצה שנמחקה של Microsoft 365 או Microsoft Teams תוך 30 יום ממחיקתה.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="8fe4f-104">עבור אל מרכז הניהול של [Microsoft 365](https://aka.ms/RestoreDeletedGroup) כדי להיכנס לרשימה של הקבוצות והצוותים שנמחקו.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="8fe4f-105">**הערה:** היכנס באמצעות החשבון שהוקצה למנהל הדייר או לתפקיד מנהל המערכת של הקבוצות.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="8fe4f-106">בחר את הקבוצה/Teams שנמחקה כדי לשחזר ולחץ על **שחזר את הקבוצה**.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="8fe4f-107">אם לא ניתן לשחזר את הקבוצה עקב כתובת SMTP מתנגשת, השתמש בפקודה הבאה כדי למצוא את האובייקט הגורם להתנגשות ולהסיר את כתובת ה- SMTP:</span><span class="sxs-lookup"><span data-stu-id="8fe4f-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="8fe4f-108">**הערה:** במקרים מסוימים, ייתכן שיקח עד 24 שעות עד שהקבוצה וכל הנתונים שלה ישוחזרו.</span><span class="sxs-lookup"><span data-stu-id="8fe4f-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="8fe4f-109">לקבלת מידע נוסף, או כדי ללמוד כיצד לשחזר קבוצות באמצעות PowerShell, ראה [שחזור קבוצה שנמחקה של Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="8fe4f-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>