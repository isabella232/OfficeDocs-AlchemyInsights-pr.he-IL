---
title: בעיות עם דיירים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7824"
- "9004325"
ms.openlocfilehash: 43f75564667bbb952076d4c12d7a1dd1e7e99731
ms.sourcegitcommit: 4e2d640a618c786700e8b276533554d51956f080
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713675"
---
# <a name="issues-with-tenants"></a><span data-ttu-id="482f8-102">בעיות עם דיירים</span><span class="sxs-lookup"><span data-stu-id="482f8-102">Issues with tenants</span></span>

<span data-ttu-id="482f8-103">תכלת Active Directory (תכלת לספירה) מארגן אובייקטים כגון משתמשים ויישומים בקבוצות שנקראות דיירים.</span><span class="sxs-lookup"><span data-stu-id="482f8-103">Azure Active Directory (Azure AD) organizes objects like users and apps into groups called tenants.</span></span> <span data-ttu-id="482f8-104">דיירים מאפשרים למנהל מערכת להגדיר מדיניות על המשתמשים בתוך הארגון ואת היישומים הנמצאים בבעלותו של הארגון כדי לעמוד במדיניות האבטחה ובמדיניות התפעולית שלהם.</span><span class="sxs-lookup"><span data-stu-id="482f8-104">Tenants allow an administrator to set policies on the users within the organization and the on apps that the organization owns to meet their security and operational policies.</span></span> <span data-ttu-id="482f8-105">לקבלת מידע נוסף, ראה [שכירות ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span><span class="sxs-lookup"><span data-stu-id="482f8-105">For more information, see [Tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span></span>

<span data-ttu-id="482f8-106">לקבלת מידע נוסף הקשור לניהול דיירים, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="482f8-106">For more information related to tenant management, see the following articles:</span></span>

- <span data-ttu-id="482f8-107">[תחלה: הגדרת דייר-מראה](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) לך כיצד ליצור דייר חדש.</span><span class="sxs-lookup"><span data-stu-id="482f8-107">[Quickstart: Set up a tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - Shows you how to create a new tenant.</span></span>

- <span data-ttu-id="482f8-108">[מחיקת דייר ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) -מראה לך כיצד למחוק דייר.</span><span class="sxs-lookup"><span data-stu-id="482f8-108">[Delete a tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - Shows you how to delete a tenant.</span></span>

<span data-ttu-id="482f8-109">**בעיות בריבוי דיירים**</span><span class="sxs-lookup"><span data-stu-id="482f8-109">**Issues with multi-tenants**</span></span>

<span data-ttu-id="482f8-110">לקבלת מידע אודות האופן שבו ניתן לנהל בעיות בנוגע לריבוי דיירים, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="482f8-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span></span>

- <span data-ttu-id="482f8-111">[כיצד לעשות זאת: היכנס למשתמש כלשהו של מדריך Active Directory באמצעות תבנית היישום ' ריבוי דיירים '](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) -מראה לך כיצד להמיר מדייר יחיד ליישום רב-דייר.</span><span class="sxs-lookup"><span data-stu-id="482f8-111">[How to: Sign in any Azure Active Directory user using the multi-tenant application pattern](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - Shows you how to convert from a single-tenant to a multi-tenant application.</span></span>
- <span data-ttu-id="482f8-112">[הגדרת כניסה עבור ארגון מסוים של תכלת Active directory ב-תכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) -מראה לך כיצד להפוך כניסה לזמינה עבור משתמשים מארגון מסוים של תכלת לספירה באמצעות זרימת משתמשים ב-תכלת AD B2C.</span><span class="sxs-lookup"><span data-stu-id="482f8-112">[Set up sign-in for a specific Azure Active Directory organization in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Shows you how to enable sign-in for users from a specific Azure AD organization using a user flow in Azure AD B2C.</span></span>
- <span data-ttu-id="482f8-113">[הגדרת כניסה עבור ריבוי דיירים של תכלת Active directory באמצעות מדיניות מותאמת אישית ב-תכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  מראה לך כיצד להפוך כניסה לזמינה עבור משתמשים באמצעות נקודת הקצה של ריבוי הדיירים עבור תכלת Active Directory (תכלת לספירה).</span><span class="sxs-lookup"><span data-stu-id="482f8-113">[Set up sign-in for multi-tenant Azure Active Directory using custom policies in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  shows you how to enable sign-in for users using the multi-tenant endpoint for Azure Active Directory (Azure AD).</span></span>






