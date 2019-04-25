---
title: הענק למשתמשים גישה SharePoint ו- OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ebb9037362d261b81b9b1dcafcbe461aac7f4963
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32400610"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="16b0d-102">הענק למשתמשים גישה SharePoint ו- OneDrive</span><span class="sxs-lookup"><span data-stu-id="16b0d-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="16b0d-103">אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שקיימת בעיית שירות זמניים.</span><span class="sxs-lookup"><span data-stu-id="16b0d-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="16b0d-104">בדוק את לוח המחוונים של שירותי בריאות</span><span class="sxs-lookup"><span data-stu-id="16b0d-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="16b0d-105">אם ברצונך שאנשים בארגון שלך כדי שתוכל להיכנס ולהשתמש SharePoint ו- OneDrive, עליך להוסיף חשבונות עבור אותם וודא כי יש להם רשיון נותן לו גישה SharePoint ו- OneDrive.</span><span class="sxs-lookup"><span data-stu-id="16b0d-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="16b0d-106">הדרך הקלה ביותר להוספת משתמשים היא במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="16b0d-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="16b0d-107">עבור אל [הדף משתמשים פעילים במרכז admin Microsoft 365](https://portal.office.com/adminportal/home#/users)ולאחר מכן לחץ על **הוסף משתמש**.</span><span class="sxs-lookup"><span data-stu-id="16b0d-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="16b0d-108">מלא את המידע עבור המשתמש, וודא כי במסגרת **רשיונות למוצר**, רשיון מוקצה **SharePoint Online** נבחרת.</span><span class="sxs-lookup"><span data-stu-id="16b0d-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="16b0d-109">שים לב כי אם תאפשר חיצוני שיתוף בארגון שלך, משתמשים יכולים לשתף תוכן SharePoint ו- OneDrive עם אנשים מחוץ לארגון.</span><span class="sxs-lookup"><span data-stu-id="16b0d-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="16b0d-110">אין צורך להעניק רשיונות משתמשים חיצוניים אלה.</span><span class="sxs-lookup"><span data-stu-id="16b0d-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="16b0d-111">גם אין צורך להוסיף חשבונות עבור אותם, אלא אם כן שיתוף מוגדר כ- "רק חיצוניים משתמשים קיימים."</span><span class="sxs-lookup"><span data-stu-id="16b0d-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="16b0d-112">במקרה זה, אם האנשים אינם בספריה של הארגון שלך, עליך להוסיף אותם כמשתמשים אורחים במרכז admin AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="16b0d-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

