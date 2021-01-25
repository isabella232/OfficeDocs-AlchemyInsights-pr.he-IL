---
title: הרשאות API והסכמה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974605"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="a1933-102">הרשאות API והסכמה</span><span class="sxs-lookup"><span data-stu-id="a1933-102">API permissions and consent</span></span>

<span data-ttu-id="a1933-103">יישומים המשולבים בפלטפורמת הזהויות של Microsoft ממלאים אחר מודל הרשאה המעניק למשתמשים ולשליטה באופן שבו ניתן לגשת לנתונים.</span><span class="sxs-lookup"><span data-stu-id="a1933-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="a1933-104">היישום של מודל ההרשאות עודכן בנקודת הקצה של פלטפורמת הזהות של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a1933-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="a1933-105">היא משנה את אופן הפעולה של האפליקציה עם פלטפורמת הזהות של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a1933-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="a1933-106">[הרשאות והסכמה בנקודת הקצה של פלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) מכסה את המושגים הבסיסיים של מודל הרשאה זה, כולל טווחים, הרשאות והסכמה.</span><span class="sxs-lookup"><span data-stu-id="a1933-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="a1933-107">[מסגרת ההסכמה של תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) מאפשרת לך לפתח בקלות יישומי אינטרנט ולקוחות מקוריים של ריבוי דיירים.</span><span class="sxs-lookup"><span data-stu-id="a1933-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="a1933-108">יישומים אלה מאפשרים כניסה על-ידי חשבונות משתמשים מדייר תכלת לספירה שונה מזה שבו היישום רשום.</span><span class="sxs-lookup"><span data-stu-id="a1933-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="a1933-109">ייתכן שתצטרך גם לגשת לממשקי Api של אינטרנט, כגון Microsoft Graph API (כדי לגשת אל התכלת לספירה, לכוונן ולשירותים ב-Microsoft 365) וממשקי Api אחרים של Microsoft services, בנוסף לממשקי ה-Api של האינטרנט שלך.</span><span class="sxs-lookup"><span data-stu-id="a1933-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

