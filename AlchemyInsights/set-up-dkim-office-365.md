---
title: התקנת DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808708"
---
# <a name="setup-dkim"></a><span data-ttu-id="ea613-102">התקנת DKIM</span><span class="sxs-lookup"><span data-stu-id="ea613-102">Setup DKIM</span></span>

<span data-ttu-id="ea613-103">ההוראות המפורטות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב-Microsoft 365 נמצאות [כאן](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="ea613-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="ea613-104">עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות CNAME של DKIM בשירות ה-dns המארח של התחום שלך (בדרך כלל, רשם התחומים).</span><span class="sxs-lookup"><span data-stu-id="ea613-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="ea613-105">לדוגמה, contoso.com ו-fourthcoffee.com דורשים ארבע רשומות CNAME של DKIM: two עבור contoso.com ושתיים עבור fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="ea613-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="ea613-106">רשומות CNAME של DKIM עבור **כל** תחום מותאם אישית משתמשות בתבניות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ea613-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="ea613-107">**שם מחשב מארח**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ea613-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ea613-108">**מצביע על כתובת או ערך**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ea613-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ea613-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="ea613-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="ea613-110">**שם מחשב מארח**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ea613-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ea613-111">**מצביע על כתובת או ערך**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ea613-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ea613-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="ea613-112">**TTL**: 3600</span></span>

   <span data-ttu-id="ea613-113">\<DomainGUID\> הוא הטקסט שמימין `.mail.protection.outlook.com` לרשומת ה-MX המותאמת אישית עבור התחום המותאם אישית (לדוגמה, `contoso-com` עבור התחום contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ea613-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="ea613-114">\<InitialDomain\> הוא התחום שבו השתמשת כאשר נרשמת ל-Microsoft 365 (לדוגמה, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="ea613-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="ea613-115">לאחר שיצרת את רשומות CNAME עבור התחומים המותאמים אישית שלך, בצע את ההוראות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ea613-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="ea613-116">מ.</span><span class="sxs-lookup"><span data-stu-id="ea613-116">a.</span></span> <span data-ttu-id="ea613-117">[היכנס ל-Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) באמצעות החשבון שלך בעבודה או בבית הספר.</span><span class="sxs-lookup"><span data-stu-id="ea613-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="ea613-118">b.</span><span class="sxs-lookup"><span data-stu-id="ea613-118">b.</span></span> <span data-ttu-id="ea613-119">בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.</span><span class="sxs-lookup"><span data-stu-id="ea613-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="ea613-120">c.</span><span class="sxs-lookup"><span data-stu-id="ea613-120">c.</span></span> <span data-ttu-id="ea613-121">בניווט הימני התחתון, הרחב את **ניהול** ובחר **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ea613-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="ea613-122">תלת.</span><span class="sxs-lookup"><span data-stu-id="ea613-122">d.</span></span> <span data-ttu-id="ea613-123">עבור אל **Protection**  >  **DKIM**Protection.</span><span class="sxs-lookup"><span data-stu-id="ea613-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="ea613-124">e.</span><span class="sxs-lookup"><span data-stu-id="ea613-124">e.</span></span> <span data-ttu-id="ea613-125">בחר את התחום ולאחר מכן בחר **הפוך לזמין** עבור **הודעות חתימה עבור תחום זה עם חתימות DKIM**.</span><span class="sxs-lookup"><span data-stu-id="ea613-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="ea613-126">חזור על שלב זה עבור כל תחום מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="ea613-126">Repeat this step for each custom domain.</span></span>
