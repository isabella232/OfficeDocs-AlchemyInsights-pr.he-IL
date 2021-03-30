---
title: קבל רשימה של יישומים ארגוניים
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404931"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="6415e-102">קבל רשימה של יישומים ארגוניים</span><span class="sxs-lookup"><span data-stu-id="6415e-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="6415e-103">כדי **לקבל רשימה של יישומים ארגוניים** (כל היישומים או מסוננים לפי שם תצוגה, מזהה, מזהי כתובות URL וכדומה) באמצעות הפקודה Powershell, ראה [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="6415e-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="6415e-104">כדי לקבל רשימה של אובייקטים ראשיים של שירות (כל האובייקטים או המסוננים לפי מזהה) באמצעות הפקודה Powershell, ראה [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="6415e-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="6415e-105">אם ברצונך לקבל רשימה **של אפליקציות המוגדרות על-ידי SAML, ייתכן שקבצי Script של PowerShell הבאים** יעזרו לך:</span><span class="sxs-lookup"><span data-stu-id="6415e-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="6415e-106">כל יישום הוא יישום OAuth או יישום SAML (הן גלריה וגם אפליקציות שאינן גלריה) כוללים שני אובייקטים שנוצרו ב- AAD כאשר הרישום שלהם מתרחש.</span><span class="sxs-lookup"><span data-stu-id="6415e-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="6415e-107">אובייקט אחד נקרא אובייקט היישום והאובייקט השני הוא האובייקט הראשי של השירות.</span><span class="sxs-lookup"><span data-stu-id="6415e-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="6415e-108">בעת השלכת המאפיינים של אובייקט ראשי של שירות באמצעות PowerShell, תגלה שלכל יישום יש מספר מסוים של תגיות המשויכות לו, כמו:</span><span class="sxs-lookup"><span data-stu-id="6415e-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="6415e-109">יישומי OAuth כוללים תגית בשם "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="6415e-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="6415e-110">אפליקציות SAML של גלריה כוללות תגית בשם "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="6415e-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="6415e-111">אפליקציות SAML שאינן גלריה כוללות תגית בשם "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="6415e-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="6415e-112">לפיכך, באפשרותך להשתמש בתגיות אלה ולברר איזה סוג יישום זה.</span><span class="sxs-lookup"><span data-stu-id="6415e-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="6415e-113">התגית "**WindowsAzureActiveDirectoryIntegratedApp**" נפוצה בכל סוגי האפליקציות.</span><span class="sxs-lookup"><span data-stu-id="6415e-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="6415e-114">באפשרותך להשתמש במקטעי הבאים כדי רשימת כל יישומי SAML (הן גלריה וגם לא גלריה):</span><span class="sxs-lookup"><span data-stu-id="6415e-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="6415e-115">לקבלת מידע נוסף, ראה [זיהוי יישומים התומכים ב- SAML ב- Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="6415e-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="6415e-116">**חיפוש ורשימה של יישומי אינטרנט בלבד:** השתמש בפקודה שלהלן כדי לקבל את כל יישומי Azure AD עם סוג היישום "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="6415e-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="6415e-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="6415e-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="6415e-118">**חפש והצג רשימה של יישומים מקוריים** בלבד: הפעל את הפקודה הבאה כדי לקבל את כל יישומי הלקוח המקורי (מחשב שולחני/מכשיר נייד).</span><span class="sxs-lookup"><span data-stu-id="6415e-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="6415e-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="6415e-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="6415e-120">**ייצא את כל פרטי היישום של Azure AD הרשומים ל- CSV**: הפקודה שלהלן מייצאת את כל יישומי Azure AD עם הפרטים הדרושים לקובץ csv:</span><span class="sxs-lookup"><span data-stu-id="6415e-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="6415e-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="6415e-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="6415e-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="6415e-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="6415e-123">**צריך לייצא רשימה של יישומים של Azure שלא נוסו** – ביקורת הדוח</span><span class="sxs-lookup"><span data-stu-id="6415e-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="6415e-124">Azure AD יכול להציג יומני יישומים עבור עד 30 יום בלבד בתנאי שיש לך רשיון Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="6415e-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="6415e-125">יש לך שתי אפשרויות לשמור את הנתונים במשך יותר מ- 30 יום.</span><span class="sxs-lookup"><span data-stu-id="6415e-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="6415e-126">באפשרותך להשתמש ב- [API של דיווח Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) כדי לאחזר את הנתונים באופן תיכנותי ולאחסן אותם במסד נתונים.</span><span class="sxs-lookup"><span data-stu-id="6415e-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="6415e-127">לחלופין, באפשרותך לשלב יומני ביקורת במערכת סיאם של ספקים שלישיים.</span><span class="sxs-lookup"><span data-stu-id="6415e-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="6415e-128">באפשרותך גם להוריד את רשימת היישומים עבור כל היישומים והיישומים שבבעלותם תחת Azure Active directory>רישום יישומים>הורד>כל היישומים/יישומים בבעלות.</span><span class="sxs-lookup"><span data-stu-id="6415e-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="6415e-129">כדי לקבל רשימה של יישומים באמצעות MS Graph, ראה רשימת יישומים [- Microsoft Graph v1.0 וסוג](https://docs.microsoft.com/graph/api/application-list) משאב יישום - Microsoft [Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="6415e-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
