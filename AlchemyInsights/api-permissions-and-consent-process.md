---
title: הרשאות API ותהליך הסכמה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404870"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="c47a9-102">הרשאות API ותהליך הסכמה</span><span class="sxs-lookup"><span data-stu-id="c47a9-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="c47a9-103">כדי שהאפליקציות שלך לגשת לנתונים ב- Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק להם את ההרשאות הנכונות באמצעות תהליך הסכמה.</span><span class="sxs-lookup"><span data-stu-id="c47a9-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="c47a9-104">[הפניה להרשאות Microsoft Graph מפרטת](https://docs.microsoft.com/graph/permissions-reference) את ההרשאות המשויכות לכל קבוצה ראשית של ממשקי API של Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c47a9-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="c47a9-105">הוא מספק גם הדרכה לגבי אופן השימוש בהרשאות.</span><span class="sxs-lookup"><span data-stu-id="c47a9-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="c47a9-106">**הגדרה או עדכון של מנהל שירות**</span><span class="sxs-lookup"><span data-stu-id="c47a9-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="c47a9-107">[יצירת serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - מאמר זה מראה לך כיצד ליצור שירות חדשאובייקטPrincipal.</span><span class="sxs-lookup"><span data-stu-id="c47a9-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="c47a9-108">[צור יישום Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) שירות ראשי בפורטל - מאמר זה מראה לך כיצד ליצור יישום חדש של Azure Active Directory (Azure AD) ומנהל שירות, איתם ניתן להשתמש עם פקד הגישה מבוסס התפקידים.</span><span class="sxs-lookup"><span data-stu-id="c47a9-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="c47a9-109">[אפליקציות &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) שירות ב- Azure AD - מאמר זה מתאר רישום יישומים, אובייקטי יישומים ומנהלי שירות ב- Azure Active Directory: מה הם, אופן השתמשו בהם ואופן הקשורים זה לזה.</span><span class="sxs-lookup"><span data-stu-id="c47a9-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="c47a9-110">**הוספה או עדכון של רישום אפליקציה וספק הסכמת מנהל מערכת**</span><span class="sxs-lookup"><span data-stu-id="c47a9-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="c47a9-111">[יצירת רישום אפליקציה](https://docs.microsoft.com/graph/api/application-post-applications) - מאמר זה מראה לך כיצד ליצור אובייקט יישום חדש.</span><span class="sxs-lookup"><span data-stu-id="c47a9-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="c47a9-112">[עדכון רישום אפליקציה - הרשאות API](https://docs.microsoft.com/graph/api/application-update) - מאמר זה מראה לך כיצד לעדכן את המאפיינים של אובייקט יישום.</span><span class="sxs-lookup"><span data-stu-id="c47a9-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="c47a9-113">[ספק הסכמת מנהל מערכת](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - לקבלת הסכמת מנהל מערכת והסכמה באופן כללי, אנו דורשים מנהל מערכת מעניק הסכמה באופן מפורש.</span><span class="sxs-lookup"><span data-stu-id="c47a9-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="c47a9-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - גורם מכיל לניהול תפקידים עבור הגדרות תפקיד מאוחדות והקצאות תפקיד עבור ספקי RBAC של Microsoft 365 התומכים במספר מנהלים וטווחים מרובים בהקצאת תפקיד בודדת.</span><span class="sxs-lookup"><span data-stu-id="c47a9-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="c47a9-115">פעולה זו שונה מסוג *המשאב rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="c47a9-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="c47a9-116">Microsoft Intune הוא דוגמה של ספק RBAC כזה.</span><span class="sxs-lookup"><span data-stu-id="c47a9-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="c47a9-117">הקצאת תפקיד ב- Intune יכולה לכוללים מערך של מנהלים ומערך של קבוצות טווח.</span><span class="sxs-lookup"><span data-stu-id="c47a9-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="c47a9-118">**אפשרות זו נמצאת בגירסת ביתא, כלומר שהיא עדיין בפיתוח ולא מומלצת לשימוש בייצור.**</span><span class="sxs-lookup"><span data-stu-id="c47a9-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
