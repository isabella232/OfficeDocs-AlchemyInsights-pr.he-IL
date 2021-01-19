---
title: פתרון בעיות בהסכמה למשתמש
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901191"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="1d750-102">פתרון בעיות בהסכמה למשתמש</span><span class="sxs-lookup"><span data-stu-id="1d750-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="1d750-103">באפשרותך לקבוע את האופן שבו משתמשי קצה מתנגדים ליישומים דרך פורטל תכלת או PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1d750-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="1d750-104">ראה [הגדרות הסכמה למשתמש](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="1d750-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="1d750-105">מנהל מערכת יכול להשתמש גם ב- [API של Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) כדי להעניק הסכמה להרשאות מוסמכות בשם משתמש יחיד.</span><span class="sxs-lookup"><span data-stu-id="1d750-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="1d750-106">לקבלת מידע נוסף, ראה [קבלת גישה בשם של משתמש](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="1d750-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="1d750-107">[שגיאות הסכמה למשתמש](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): מאמר זה דן בשגיאות שעלולות להתרחש במהלך תהליך ההסכמה ליישום.</span><span class="sxs-lookup"><span data-stu-id="1d750-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="1d750-108">אם אתה פותר בקשות להסכמה בלתי צפויות שאינן מכילות הודעות שגיאה, ראה [תרחישי אימות עבור תכלת לספירה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="1d750-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>