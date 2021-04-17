---
title: כיצד להפוך SSO חלק לזמין
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825732"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="924a9-102">כיצד להפוך SSO חלק לזמין</span><span class="sxs-lookup"><span data-stu-id="924a9-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="924a9-103">הפוך SSO חלק לזמין באמצעות [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="924a9-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="924a9-104">אם אתה עושה התקנה חדשה של Azure AD Connect, בחר את נתיב ההתקנה [המותאם אישית](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="924a9-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="924a9-105">בדף **הכניסה של המשתמש,** בחר באפשרות **הפוך כניסה יחידה לזמינה.**</span><span class="sxs-lookup"><span data-stu-id="924a9-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="924a9-106">כדי לוודא שהאפשרות חלקה SSO נכונה:</span><span class="sxs-lookup"><span data-stu-id="924a9-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="924a9-107">היכנס למרכז הניהול [של Azure Active Directory כמנהל](https://aad.portal.azure.com) מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="924a9-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="924a9-108">בחר **Azure Active Directory** בחלונית הימנית.</span><span class="sxs-lookup"><span data-stu-id="924a9-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="924a9-109">ודא שהכניסה יחידה חלקה **זמינה.**</span><span class="sxs-lookup"><span data-stu-id="924a9-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="924a9-110">כדי ללמוד עוד, ראה [כניסה יחידה חלקה של Azure Active Directory: התחלה מהירה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="924a9-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  