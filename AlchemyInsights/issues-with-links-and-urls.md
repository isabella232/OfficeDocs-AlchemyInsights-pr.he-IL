---
title: בעיות עם קישורים וכתובות Url
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974465"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="adb9a-102">בעיות עם קישורים וכתובות Url</span><span class="sxs-lookup"><span data-stu-id="adb9a-102">Issues with links and URLs</span></span>

<span data-ttu-id="adb9a-103">ניתוב מחדש של כתובות Url של URI/השב (שני הביטויים הם להחלפה) הם כתובות ה-Url המשמשות את פלטפורמת הזהויות של Microsoft כדי להחזיר אסימונים המבוקשים על-ידי יישום.</span><span class="sxs-lookup"><span data-stu-id="adb9a-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="adb9a-104">לקבלת מידע על כתובות Url אלה, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="adb9a-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="adb9a-105">[זרימות אימות ותרחישים של יישומים](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -מידע אודות הניתוב מחדש של רכיבי uri בדף **ההרשמה של האפליקציה** עבור כל תרחיש.</span><span class="sxs-lookup"><span data-stu-id="adb9a-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="adb9a-106">ניתוב מחדש של הגבלות ומגבלות של כתובות URL של URI</span><span class="sxs-lookup"><span data-stu-id="adb9a-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="adb9a-107">**איני יודע כיצד לרשום את כתובת ה-URL הנכונה של URI/השב עבור היישום שלי**</span><span class="sxs-lookup"><span data-stu-id="adb9a-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="adb9a-108">בעת הכניסה באמצעות היישום שאתה מפתח, אם תיבת הדו של הכניסה מציגה את **AADSTS50011: כתובת ה-url שצוינה בבקשה אינה תואמת לכתובות ה-url של התשובה שתצורתן נקבעה עבור היישום <your app ID>**, יהיה עליך להוסיף לרישום היישומים שלך, ה-URI המנתב המשמש את הקוד בבקשת האסימון לפלטפורמת ה</span><span class="sxs-lookup"><span data-stu-id="adb9a-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="adb9a-109">כדי להוסיף כתובת URL של תשובה, עבור אל הכרטיסיה **אימות** בדף **הרישום של היישום** בפורטל תכלת והוסף ערך במקטע **ניתוב מחדש של רכיבי uri** .</span><span class="sxs-lookup"><span data-stu-id="adb9a-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="adb9a-110">כתובות Uri של ניתוב מחדש מוקלדות (אינטרנט או מחשב נייד/שולחן עבודה).</span><span class="sxs-lookup"><span data-stu-id="adb9a-110">Redirect URIs are typed (Web or mobile/desktop).</span></span> <span data-ttu-id="adb9a-111">הערך שעליך להזין תלוי בסוג היישום שאתה בונה, כמתואר להלן:</span><span class="sxs-lookup"><span data-stu-id="adb9a-111">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="adb9a-112">עבור יישומים בעלי עמוד אחד ויישומי אינטרנט, כתובת ה-URL של התשובה היא כתובת URL ביישום שלך.</span><span class="sxs-lookup"><span data-stu-id="adb9a-112">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="adb9a-113">ראה [רישום יישומים בעלי עמוד אחד](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) או [רישום יישום web app באמצעות פורטל תכלת](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="adb9a-113">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="adb9a-114">עבור יישומי שולחן העבודה, הערך שעליך לבחור תלוי ב:</span><span class="sxs-lookup"><span data-stu-id="adb9a-114">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="adb9a-115">הפלטפורמה (MacOS שונה מ-Windows או Linux)</span><span class="sxs-lookup"><span data-stu-id="adb9a-115">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="adb9a-116">האופן שבו אתה רוכש את האסימון (באופן אינטראקטיבי, עם זרימת קוד מכשיר, עם אימות משולב של Windows [של יווה] או עם שם משתמש/סיסמה).</span><span class="sxs-lookup"><span data-stu-id="adb9a-116">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="adb9a-117">לקבלת פרטים, ראה [יישומי שולחן עבודה-רישום יישומים-ניתוב מחדש של URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="adb9a-117">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="adb9a-118">עבור אפליקציות למכשירים ניידים, אורי הניתוב מחדש תלוי ב:</span><span class="sxs-lookup"><span data-stu-id="adb9a-118">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="adb9a-119">הפלטפורמה (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="adb9a-119">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="adb9a-120">המידע המשמש לבניית האפליקציה שלך, כגון מזהה החבילה ב-iOS, ושם החבילה וקוד ה-hash של החתימה במכשיר Android הרישום של אפליקציית הפורטל תכלת יסייע לך.</span><span class="sxs-lookup"><span data-stu-id="adb9a-120">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="adb9a-121">לקבלת פרטים, ראה [תצורת פלטפורמה וניתוב מחדש של רכיבי uri](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="adb9a-121">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="adb9a-122">ממשקי Api של אינטרנט וחלק מהדרכים השקטה של רכישת אסימונים (של יווה ו-username/password) אינם דורשים מחדש URI.</span><span class="sxs-lookup"><span data-stu-id="adb9a-122">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="adb9a-123">**פרסת את יישום האינטרנט שלי וכאשר אני מבדוק את האפליקציה שנפרסת, אני מקבל הודעת אי התאמה של כתובת url של תשובה**</span><span class="sxs-lookup"><span data-stu-id="adb9a-123">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="adb9a-124">הוסף רכיבי Uri של ניתוב מחדש עבור כל המיקומים שבהם אתה מפרוס את יישום האינטרנט שלך.</span><span class="sxs-lookup"><span data-stu-id="adb9a-124">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="adb9a-125">לקבלת מידע נוסף, ראה [רישום יישום web app באמצעות פורטל התכלת](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="adb9a-125">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="adb9a-126">הוסף את URI לניתוב מחדש עבור מיקום מיד לאחר שפרסת את היישום במיקום זה.</span><span class="sxs-lookup"><span data-stu-id="adb9a-126">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="adb9a-127">**איני מצליח לרשום מספיק כתובות Url של תשובות**</span><span class="sxs-lookup"><span data-stu-id="adb9a-127">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="adb9a-128">אתה משתמש ב-ISV וברשותך מספר כתובות ניתוב מחדש לניתוב מחדש עבור כל לקוח שלך.</span><span class="sxs-lookup"><span data-stu-id="adb9a-128">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="adb9a-129">ברצונך להעביר מ-ADAL/תכלת AD v 1.0 ל-MSAL/פלטפורמת הזהויות של Microsoft והגעת [למספר המרבי של רכיבי uri של ניתוב מחדש](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="adb9a-129">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="adb9a-130">כדי לפתור זאת, [הוסף מחדש רכיבי uri למנהלי שירות](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) המתאימים לכל אחד מהלקוחות שלך.</span><span class="sxs-lookup"><span data-stu-id="adb9a-130">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
