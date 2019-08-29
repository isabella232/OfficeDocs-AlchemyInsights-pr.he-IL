---
title: כיצד לאפשר SSO חלקה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 3cf751bc42322067c4b7cd9b5facb933430f2b87
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36663863"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="16772-102">כיצד לאפשר SSO חלקה</span><span class="sxs-lookup"><span data-stu-id="16772-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="16772-103">אפשר SSO חלקה באמצעות [AD תכלת הרקיע להתחבר](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="16772-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="16772-104">אם אתה מבצע התקנה חדשה של התחברות AD תכלת הרקיע, לבחור את [נתיב ההתקנה המותאמת אישית](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="16772-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="16772-105">בדף **משתמש כניסה** , בחר באפשרות **אפשר כניסה יחידה** .</span><span class="sxs-lookup"><span data-stu-id="16772-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="16772-106">כדי לוודא כי הפכת SSO חלקה כראוי:</span><span class="sxs-lookup"><span data-stu-id="16772-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="16772-107">היכנס אל [מרכז ניהול תכלת הרקיע Active Directory](https://aad.portal.azure.com) בתור מנהל מערכת כללית</span><span class="sxs-lookup"><span data-stu-id="16772-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="16772-108">בחר **תכלת הרקיע Active Directory** בחלונית הימנית.</span><span class="sxs-lookup"><span data-stu-id="16772-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="16772-109">ודא זה חלקה כניסה יחידה **זמין**.</span><span class="sxs-lookup"><span data-stu-id="16772-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="16772-110">לקבלת מידע נוסף, ראה [תכלת הרקיע Active Directory חלקה כניסה יחידה: התחלה מהירה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="16772-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  