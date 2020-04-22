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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645673"
---
# <a name="setup-dkim"></a><span data-ttu-id="edbf9-102">הגדרת DKIM</span><span class="sxs-lookup"><span data-stu-id="edbf9-102">Setup DKIM</span></span>

<span data-ttu-id="edbf9-103">ההנחיות השלמות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב-Microsoft 365 נמצאים [כאן](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="edbf9-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="edbf9-104">עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות של dkim CNAME בשירות ה-DNS המארח של התחום שלך (בדרך כלל, רשם התחום).</span><span class="sxs-lookup"><span data-stu-id="edbf9-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="edbf9-105">לדוגמה, contoso.com ו-fourthcoffee.com דורשות ארבע רשומות של DKIM CNAME: שתיים עבור contoso.com ושתיים עבור fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="edbf9-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="edbf9-106">רשומות ה-DKIM CNAME עבור **כל** תחום מותאם אישית משתמשות בתבניות הבאות:</span><span class="sxs-lookup"><span data-stu-id="edbf9-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="edbf9-107">**שם מחשב מארח**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="edbf9-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="edbf9-108">**נקודות לכתובת או לערך**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="edbf9-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="edbf9-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="edbf9-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="edbf9-110">**שם מחשב מארח**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="edbf9-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="edbf9-111">**נקודות לכתובת או לערך**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="edbf9-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="edbf9-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="edbf9-112">**TTL**: 3600</span></span>

   <span data-ttu-id="edbf9-113">\<DomainGUID\> הוא הטקסט שמשמאל `.mail.protection.outlook.com` לרשומת ה-MX המותאמת אישית עבור קבוצת המחשבים המותאמת אישית `contoso-com` (לדוגמה, עבור קבוצת המחשבים contoso.com).</span><span class="sxs-lookup"><span data-stu-id="edbf9-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="edbf9-114">\<אתחאלתחום\> הוא התחום שבו השתמשת כאשר נרשמת ל365 של Microsoft (לדוגמה, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="edbf9-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="edbf9-115">לאחר שיצרת את רשומות ה-CNAME עבור התחומים המותאמים אישית שלך, השלם את ההוראות הבאות:</span><span class="sxs-lookup"><span data-stu-id="edbf9-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="edbf9-116">קצת.</span><span class="sxs-lookup"><span data-stu-id="edbf9-116">a.</span></span> <span data-ttu-id="edbf9-117">[היכנס ל-Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) עם העבודה שלך או חשבון בית הספר.</span><span class="sxs-lookup"><span data-stu-id="edbf9-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="edbf9-118">b.</span><span class="sxs-lookup"><span data-stu-id="edbf9-118">b.</span></span> <span data-ttu-id="edbf9-119">בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.</span><span class="sxs-lookup"><span data-stu-id="edbf9-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="edbf9-120">c.</span><span class="sxs-lookup"><span data-stu-id="edbf9-120">c.</span></span> <span data-ttu-id="edbf9-121">בניווט השמאלי התחתון, הרחב את **Admin** ובחר באפשרות **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="edbf9-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="edbf9-122">d.</span><span class="sxs-lookup"><span data-stu-id="edbf9-122">d.</span></span> <span data-ttu-id="edbf9-123">. לך **להגנה** > **.**</span><span class="sxs-lookup"><span data-stu-id="edbf9-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="edbf9-124">e.</span><span class="sxs-lookup"><span data-stu-id="edbf9-124">e.</span></span> <span data-ttu-id="edbf9-125">בחר את התחום ולאחר מכן בחר **באפשרות ' הפעל** **הודעות ' עבור תחום זה עם חתימות dkim**.</span><span class="sxs-lookup"><span data-stu-id="edbf9-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="edbf9-126">חזור על שלב זה עבור כל תחום מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="edbf9-126">Repeat this step for each custom domain.</span></span>
