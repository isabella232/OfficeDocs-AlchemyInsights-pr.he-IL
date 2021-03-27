---
title: היכנס ל- Microsoft Edge באופן אוטומטי
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398730"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="e6d9a-102">היכנס ל- Microsoft Edge באופן אוטומטי</span><span class="sxs-lookup"><span data-stu-id="e6d9a-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="e6d9a-103">Microsoft Edge משתמש בחשבון ברירת המחדל של מערכת ההפעלה כדי להיכנס באופן אוטומטי למשתמש בהתאם לתצורה של המכשיר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="e6d9a-104">התרחישים של כל סוג של תצורת מכשיר ותהליך הכניסה של המשתמש התלוי שלו מתוארים להלן:</span><span class="sxs-lookup"><span data-stu-id="e6d9a-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="e6d9a-105">**המכשיר הוא היברידי/AAD-J:** אפשרות זו זמינה ב- Windows 10, ב- Windows ברמה נמוכה ובגרסאות שרת תואמות.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="e6d9a-106">המשתמשים מחוברים באופן אוטומטי באמצעות חשבונות Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="e6d9a-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="e6d9a-107">**המכשיר מצורף לתחום**: אפשרות זו זמינה ב- Windows 10, ב- Windows ברמה נמוכה ובגרסאות שרת תואמות.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="e6d9a-108">כברירת מחדל, משתמשים בעלי חשבונות תחום אינם מחוברים באופן אוטומטי; כדי להפוך כניסה אוטומטית לזמינה עבורם, השתמש במדיניות **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="e6d9a-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="e6d9a-109">כדי להפוך כניסה אוטומטית לזמינה עבור משתמשים בעלי חשבונות Azure AD, שקול להצטרף באופן היברידי למכשירים שלהם.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="e6d9a-110">**חשבון ברירת** המחדל של מערכת ההפעלה הוא חשבון Microsoft : אפשרות זו זמינה ב- Windows 10 RS3 (גירסה 1709, גירסת Build מס' 10.0.16299) וגירסאות מתקדמות יותר.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="e6d9a-111">לא סביר שהתרחיש יתרחש במכשירים ארגוניים.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="e6d9a-112">עם זאת, אם חשבון ברירת המחדל של מערכת ההפעלה הוא חשבון Microsoft, Microsoft Edge יחתום באופן אוטומטי על המשתמש באמצעות חשבון Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e6d9a-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
