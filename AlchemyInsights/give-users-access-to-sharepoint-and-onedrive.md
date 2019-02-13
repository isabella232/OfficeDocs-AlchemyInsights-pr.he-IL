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
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 8984d8dfdd8f1ff540b418dfbfe382cffac978e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29933841"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="21fd1-102">הענק למשתמשים גישה SharePoint ו- OneDrive</span><span class="sxs-lookup"><span data-stu-id="21fd1-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="21fd1-p101">אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שקיימת בעיית שירות זמניים. [בדוק את לוח המחוונים של שירותי בריאות](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="21fd1-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="21fd1-p102">אם ברצונך שאנשים בארגון שלך כדי שתוכל להיכנס ולהשתמש SharePoint ו- OneDrive, עליך להוסיף חשבונות עבור אותם וודא כי יש להם רשיון נותן לו גישה SharePoint ו- OneDrive. הדרך הקלה ביותר להוספת משתמשים היא במרכז הניהול של Office 365.</span><span class="sxs-lookup"><span data-stu-id="21fd1-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="21fd1-107">עבור אל [הדף משתמשים פעילים במרכז הניהול של Office 365](https://portal.office.com/adminportal/home#/users), ולאחר מכן לחץ על **הוסף משתמש**.</span><span class="sxs-lookup"><span data-stu-id="21fd1-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="21fd1-108">מלא את המידע עבור המשתמש, וודא כי במסגרת **רשיונות למוצר**, רשיון מוקצה **SharePoint Online** נבחרת.</span><span class="sxs-lookup"><span data-stu-id="21fd1-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="21fd1-p103">שים לב כי אם תאפשר חיצוני שיתוף בארגון שלך, משתמשים יכולים לשתף תוכן SharePoint ו- OneDrive עם אנשים מחוץ לארגון. אין צורך להעניק רשיונות משתמשים חיצוניים אלה. גם אין צורך להוסיף חשבונות עבור אותם, אלא אם כן שיתוף מוגדר כ- "רק חיצוניים משתמשים קיימים." במקרה זה, אם האנשים אינם בספריה של הארגון שלך, עליך להוסיף אותם כמשתמשים אורחים במרכז admin AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="21fd1-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

