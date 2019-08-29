---
title: עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665761"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="6f0b9-102">עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי</span><span class="sxs-lookup"><span data-stu-id="6f0b9-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="6f0b9-103">במרכז הניהול של Microsoft 365, לעבור לתוכנית **ההתקנה** > [תחומים](https://portal.office.com/adminportal/home#/Domains) עמוד, ובחר ברשימת התחומים, התחום בו אתה משתמש עבור אתר האינטרנט שלך.</span><span class="sxs-lookup"><span data-stu-id="6f0b9-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="6f0b9-104">בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="6f0b9-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="6f0b9-105">עבור **סוג DNS** הזן: **A (כתובת)**</span><span class="sxs-lookup"><span data-stu-id="6f0b9-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="6f0b9-106">עבור **שם מארח או כינוי**, הקלד: **@**</span><span class="sxs-lookup"><span data-stu-id="6f0b9-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="6f0b9-107">עבור **כתובת IP**, הקלד את כתובת ה- IP הסטטית עבור אתר האינטרנט שלך במקום שבו הוא מתארח כעת (לדוגמה, 172.16.140.1‏).</span><span class="sxs-lookup"><span data-stu-id="6f0b9-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="6f0b9-p101">כתובת זו חייבת להיות כתובת IP  *סטטית*  עבור אתר האינטרנט, ולא כתובת IP  *דינאמית*  . בדוק באתר שבו מתארח אתר האינטרנט שלך כדי לוודא שבאפשרותך לקבל כתובת IP סטטית עבור אתר האינטרנט הציבורי.</span><span class="sxs-lookup"><span data-stu-id="6f0b9-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="6f0b9-110">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6f0b9-110">Select **Save**.</span></span>

<span data-ttu-id="6f0b9-111">ניתן גם ליצור רשומת CNAME כדי לעזור למבקרים למצוא את אתר האינטרנט שלך.</span><span class="sxs-lookup"><span data-stu-id="6f0b9-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="6f0b9-112">בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="6f0b9-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="6f0b9-113">עבור **סוג DNS** הזן: **CNAME (כינוי)‎**</span><span class="sxs-lookup"><span data-stu-id="6f0b9-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="6f0b9-114">עבור **שם מארח או כינוי**, הקלד: **www**</span><span class="sxs-lookup"><span data-stu-id="6f0b9-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="6f0b9-115">עבור **כתובת מפנה**, הקלד את שם התחום המלא (FQDN) של אתר האינטרנט שלך (לדוגמה, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6f0b9-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="6f0b9-116">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6f0b9-116">Select **Save**.</span></span>
