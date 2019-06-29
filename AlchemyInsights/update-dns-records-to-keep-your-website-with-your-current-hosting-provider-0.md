---
title: עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353178"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="ff6e2-102">עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי</span><span class="sxs-lookup"><span data-stu-id="ff6e2-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="ff6e2-103">בדף [תחומים](https://portal.office.com/adminportal/home#/Domains), ברשימת התחומים, בחר את התחום שבו אתה משתמש עבור אתר האינטרנט שלך ולאחר מכן בחר **הגדרות DNS** בחלונית הניהול.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="ff6e2-104">בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="ff6e2-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ff6e2-105">עבור **סוג DNS** הזן: **A (כתובת)**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="ff6e2-106">עבור **שם מארח או כינוי**, הקלד: **@**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="ff6e2-107">עבור **כתובת IP**, הקלד את כתובת ה- IP הסטטית עבור אתר האינטרנט שלך במקום שבו הוא מתארח כעת (לדוגמה, 172.16.140.1‏).</span><span class="sxs-lookup"><span data-stu-id="ff6e2-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="ff6e2-p101">כתובת זו חייבת להיות כתובת IP  *סטטית*  עבור אתר האינטרנט, ולא כתובת IP  *דינאמית*  . בדוק באתר שבו מתארח אתר האינטרנט שלך כדי לוודא שבאפשרותך לקבל כתובת IP סטטית עבור אתר האינטרנט הציבורי.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="ff6e2-110">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-110">Select **Save**.</span></span>

<span data-ttu-id="ff6e2-111">ניתן גם ליצור רשומת CNAME כדי לעזור למבקרים למצוא את אתר האינטרנט שלך.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="ff6e2-112">בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="ff6e2-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ff6e2-113">עבור **סוג DNS** הזן: **CNAME (כינוי)‎**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="ff6e2-114">עבור **שם מארח או כינוי**, הקלד: **www**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="ff6e2-115">עבור **כתובת מפנה**, הקלד את שם התחום המלא (FQDN) של אתר האינטרנט שלך (לדוגמה, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ff6e2-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="ff6e2-116">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-116">Select **Save**.</span></span>
