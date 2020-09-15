---
title: הענקת גישה למשתמשים ל-SharePoint ו-OneDrive
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
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677208"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="eb08e-102">הענקת גישה למשתמשים ל-SharePoint ו-OneDrive</span><span class="sxs-lookup"><span data-stu-id="eb08e-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="eb08e-103">אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיו ברשותם גישה בעבר, ייתכן שקיימת בעיה של שירות זמני.</span><span class="sxs-lookup"><span data-stu-id="eb08e-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="eb08e-104">בדיקת לוח המחוונים של תקינות השירות</span><span class="sxs-lookup"><span data-stu-id="eb08e-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="eb08e-105">אם ברצונך שאנשים בארגון שלך יוכלו להיכנס ולהשתמש ב-SharePoint וב-OneDrive, עליך להוסיף חשבונות עבורם ולוודא שיש להם רשיון המעניק להם גישה ל-SharePoint ול-OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eb08e-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="eb08e-106">הדרך הקלה ביותר להוספת משתמשים היא במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eb08e-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="eb08e-107">עבור אל [הדף משתמשים פעילים במרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/users)ולאחר מכן לחץ על **הוסף משתמש**.</span><span class="sxs-lookup"><span data-stu-id="eb08e-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="eb08e-108">מלא את המידע עבור המשתמש ולאחר מכן ודא שתחת **רשיונות מוצר**, הוקצה רשיון ו- **SharePoint Online** נבחר.</span><span class="sxs-lookup"><span data-stu-id="eb08e-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="eb08e-109">שים לב שאם תאפשר שיתוף חיצוני בארגון שלך, משתמשים יוכלו לשתף תוכן של SharePoint ו-OneDrive עם אנשים מחוץ לארגון.</span><span class="sxs-lookup"><span data-stu-id="eb08e-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="eb08e-110">אין צורך להעניק רשיונות משתמשים חיצוניים אלה.</span><span class="sxs-lookup"><span data-stu-id="eb08e-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="eb08e-111">כמו כן, אין צורך להוסיף חשבונות עבורם, אלא אם האפשרות שיתוף מוגדרת ל-"משתמשים חיצוניים קיימים בלבד".</span><span class="sxs-lookup"><span data-stu-id="eb08e-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="eb08e-112">במקרה זה, אם האנשים אינם מופיעים במדריך הכתובות של הארגון שלך, עליך להוסיף אותם כמשתמשים אורחים במרכז הניהול של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="eb08e-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

