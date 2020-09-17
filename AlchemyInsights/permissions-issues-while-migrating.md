---
title: בעיות בהרשאות בעת העברה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 39b36a85319ccd71278571f3a3cbbc7cf0b9f0fa
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798053"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="b643f-102">פרופיל משתמש וסינכרון תמונות</span><span class="sxs-lookup"><span data-stu-id="b643f-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="b643f-103">**סינכרון תמונות של פרופילים** -משתמשים עשויים להבחין בכך שתמונת הפרופיל שלהם אינה מסתנכרן עם SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b643f-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="b643f-104">לחלופין, ייתכן שניסו לעדכן את תמונת הפרופיל שלהם והתמונה עדיין מופיעה כתמונה הישנה.</span><span class="sxs-lookup"><span data-stu-id="b643f-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="b643f-105">כדי להבטיח שתמונת הפרופיל תופיע כצפוי, המשתמש יצטרך ליזום סינכרון תמונות.</span><span class="sxs-lookup"><span data-stu-id="b643f-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="b643f-106">לקבלת מידע נוסף אודות תהליך סינכרון התמונות, ראה [מידע אודות סינכרון תמונות של פרופיל ב-Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="b643f-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="b643f-107">**סינכרון פרופילים** -הזמן הנדרש להשלמת סינכרון פרופילים תלוי במספר השינויים (עבודה) שמשימת הייבוא של AD צריכה להתבצע.</span><span class="sxs-lookup"><span data-stu-id="b643f-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="b643f-108">אם יש שינויים רבים, משימת שעון העצר מתבצעת בעבודה רבה, והשינויים יימשך זמן רב יותר לשינוי השינויים ביישום פרופיל המשתמש.</span><span class="sxs-lookup"><span data-stu-id="b643f-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="b643f-109">אם משימת שעון העצר כוללת נפח עבודה קטן, השינויים ישתקפו ביישום פרופילי המשתמשים במהירות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="b643f-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="b643f-110">לקבלת מידע נוסף אודות תהליך סינכרון הפרופילים, ראה [מידע אודות סינכרון פרופילי משתמשים ב-SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="b643f-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="b643f-111">**עדכון פרופיל ב-Office** לצורך התרחבות משתמשים יכולים לנהל את הפרופיל שלהם ב-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b643f-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="b643f-112">לקבלת מידע נוסף, ראה [הצגה ועדכון של הפרופיל שלך ב-Office](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)איכסון.</span><span class="sxs-lookup"><span data-stu-id="b643f-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

