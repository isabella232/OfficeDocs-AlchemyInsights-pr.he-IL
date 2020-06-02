---
title: הגדרת DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509385"
---
# <a name="setup-dkim"></a><span data-ttu-id="79742-102">הגדרת DKIM</span><span class="sxs-lookup"><span data-stu-id="79742-102">Setup DKIM</span></span>

<span data-ttu-id="79742-103">ההנחיות השלמות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב-Microsoft 365 נמצאים [כאן](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="79742-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="79742-104">עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות של dkim CNAME בשירות ה-DNS המארח של התחום שלך (בדרך כלל, רשם התחום).</span><span class="sxs-lookup"><span data-stu-id="79742-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="79742-105">לדוגמה, contoso.com ו-fourthcoffee.com דורשות ארבע רשומות של DKIM CNAME: שתיים עבור contoso.com ושתיים עבור fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="79742-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="79742-106">רשומות ה-DKIM CNAME עבור **כל** תחום מותאם אישית משתמשות בתבניות הבאות:</span><span class="sxs-lookup"><span data-stu-id="79742-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="79742-107">**שם מחשב מארח**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="79742-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="79742-108">**נקודות לכתובת או לערך**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="79742-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="79742-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="79742-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="79742-110">**שם מחשב מארח**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="79742-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="79742-111">**נקודות לכתובת או לערך**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="79742-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="79742-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="79742-112">**TTL**: 3600</span></span>

   <span data-ttu-id="79742-113">\<DomainGUID\>הוא הטקסט שמשמאל `.mail.protection.outlook.com` לרשומת ה-MX המותאמת אישית עבור התחום המותאם אישית (לדוגמה, `contoso-com` עבור התחום contoso.com).</span><span class="sxs-lookup"><span data-stu-id="79742-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="79742-114">\<InitialDomain\>הוא התחום בו השתמשת כאשר נרשמת עבור Microsoft 365 (לדוגמה, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="79742-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="79742-115">לאחר שיצרת את רשומות ה-CNAME עבור התחומים המותאמים אישית שלך, השלם את ההוראות הבאות:</span><span class="sxs-lookup"><span data-stu-id="79742-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="79742-116">קצת.</span><span class="sxs-lookup"><span data-stu-id="79742-116">a.</span></span> <span data-ttu-id="79742-117">[היכנס ל-Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) עם העבודה שלך או חשבון בית הספר.</span><span class="sxs-lookup"><span data-stu-id="79742-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="79742-118">b.</span><span class="sxs-lookup"><span data-stu-id="79742-118">b.</span></span> <span data-ttu-id="79742-119">בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.</span><span class="sxs-lookup"><span data-stu-id="79742-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="79742-120">c.</span><span class="sxs-lookup"><span data-stu-id="79742-120">c.</span></span> <span data-ttu-id="79742-121">בניווט השמאלי התחתון, הרחב את **Admin** ובחר באפשרות **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="79742-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="79742-122">d.</span><span class="sxs-lookup"><span data-stu-id="79742-122">d.</span></span> <span data-ttu-id="79742-123">. לך **להגנה**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="79742-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="79742-124">e.</span><span class="sxs-lookup"><span data-stu-id="79742-124">e.</span></span> <span data-ttu-id="79742-125">בחר את התחום ולאחר מכן בחר **באפשרות ' הפעל** **הודעות ' עבור תחום זה עם חתימות dkim**.</span><span class="sxs-lookup"><span data-stu-id="79742-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="79742-126">חזור על שלב זה עבור כל תחום מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="79742-126">Repeat this step for each custom domain.</span></span>
