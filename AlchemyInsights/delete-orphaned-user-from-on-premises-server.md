---
title: מחק משתמש יתום מהשרת המקומי
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198184"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="08b76-102">מחק משתמש יתום מהשרת המקומי</span><span class="sxs-lookup"><span data-stu-id="08b76-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="08b76-103">כדי להסיר משתמש יתום, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="08b76-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="08b76-104">אלץ סינכרון ספריות על-ידי ביצוע ההוראות ב- [מהי זהות היברידית עם הספריה הפעילה התכלת?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="08b76-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="08b76-105">כדי לאמת את סינכרון הספריות, ראה [מהי זהות היברידית באמצעות המדריך הפעיל?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="08b76-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="08b76-106">אם הסינכרון מתפקד כראוי אך מחיקת האובייקטים של Active Directory אינה מופצות לתכלת, הסר את האובייקט היתום באופן ידני באמצעות אחד ממודולי הספריה הבאה של הכלי הפעיל עבור יישומוני cmdlet של Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="08b76-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="08b76-107">הסר-מסולאיש קשר</span><span class="sxs-lookup"><span data-stu-id="08b76-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="08b76-108">הסר-מקבוצת מולטי</span><span class="sxs-lookup"><span data-stu-id="08b76-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="08b76-109">הסר-MsolUser</span><span class="sxs-lookup"><span data-stu-id="08b76-109">Remove-MsolUser</span></span>

    <span data-ttu-id="08b76-110">לדוגמה, כדי להסיר john.smith@contoso.com מזהה משתמש יתום, שנוצר במקור באמצעות סינכרון ספריות, הפעל את ה-cmdlet:</span><span class="sxs-lookup"><span data-stu-id="08b76-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="08b76-111">הסר-MsolUser-משתמש הJohn.Smith@Contoso.com שם</span><span class="sxs-lookup"><span data-stu-id="08b76-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>