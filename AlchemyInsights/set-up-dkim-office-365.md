---
title: ההתקנה DKIM ב- Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765121"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="e41b3-102">ההתקנה DKIM ב- Office 365</span><span class="sxs-lookup"><span data-stu-id="e41b3-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="e41b3-103">הוראות מלאות עבור קביעת תצורה של DKIM עבור תחומים מותאמים אישית ב- Office 365 הם [כאן](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="e41b3-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="e41b3-104">עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות DKIM CNAME בכל לשירות אירוח ה-DNS של התחום שלך (בדרך כלל, רשם תחום).</span><span class="sxs-lookup"><span data-stu-id="e41b3-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="e41b3-105">לדוגמה, contoso.com fourthcoffee.com דורשים ארבע רשומות DKIM CNAME: שני עבור contoso.com ומשני עבור fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="e41b3-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="e41b3-106">רשומות DKIM CNAME עבור **כל** תחום מותאם אישית להשתמש בתבניות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e41b3-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="e41b3-107">**שם המחשב המארח**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e41b3-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e41b3-108">**נקודות לכתובת או ערך**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e41b3-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e41b3-109">**אורך חיים**: 3600</span><span class="sxs-lookup"><span data-stu-id="e41b3-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="e41b3-110">**שם המחשב המארח**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e41b3-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e41b3-111">**נקודות לכתובת או ערך**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e41b3-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e41b3-112">**אורך חיים**: 3600</span><span class="sxs-lookup"><span data-stu-id="e41b3-112">**TTL**: 3600</span></span>

   <span data-ttu-id="e41b3-113">\<DomainGUID\> טקסט מימין `.mail.protection.outlook.com` ברשומת MX מותאם אישית עבור התחום המותאם אישית (לדוגמה, `contoso-com` עבור contoso.com תחום).</span><span class="sxs-lookup"><span data-stu-id="e41b3-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="e41b3-114">\<InitialDomain\> הוא התחום שבו השתמשת כאשר נרשמת לקבלת Office 365 (לדוגמה, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="e41b3-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="e41b3-115">לאחר שיצרת את רשומות CNAME לתחומים המותאם אישית שלך, בצע את ההוראות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e41b3-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="e41b3-116">a.</span><span class="sxs-lookup"><span data-stu-id="e41b3-116">a.</span></span> <span data-ttu-id="e41b3-117">[היכנס ל- Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) באמצעות חשבון בעבודה או בבית ספר השייך לך.</span><span class="sxs-lookup"><span data-stu-id="e41b3-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="e41b3-118">b.</span><span class="sxs-lookup"><span data-stu-id="e41b3-118">b.</span></span> <span data-ttu-id="e41b3-119">בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.</span><span class="sxs-lookup"><span data-stu-id="e41b3-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="e41b3-120">c.</span><span class="sxs-lookup"><span data-stu-id="e41b3-120">c.</span></span> <span data-ttu-id="e41b3-121">בחלונית הניווט הימנית התחתונה, הרחב **Admin** ובחר **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e41b3-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="e41b3-122">d.</span><span class="sxs-lookup"><span data-stu-id="e41b3-122">d.</span></span> <span data-ttu-id="e41b3-123">עבור אל **הגנה** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="e41b3-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="e41b3-124">e.</span><span class="sxs-lookup"><span data-stu-id="e41b3-124">e.</span></span> <span data-ttu-id="e41b3-125">בחר את התחום ולאחר מכן בחר **לזמינה** עבור **הודעות כניסה עבור קבוצת מחשבים זו עם חתימות DKIM**.</span><span class="sxs-lookup"><span data-stu-id="e41b3-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="e41b3-126">חזור על שלב זה עבור כל תחום מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="e41b3-126">Repeat this step for each custom domain.</span></span>
