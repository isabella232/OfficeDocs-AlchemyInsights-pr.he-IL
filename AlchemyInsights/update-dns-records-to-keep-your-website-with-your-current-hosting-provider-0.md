---
title: עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292173"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="5b471-102">עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי</span><span class="sxs-lookup"><span data-stu-id="5b471-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="5b471-103">בדף [תחומים](https://portal.office.com/adminportal/home#/Domains), ברשימת התחומים, בחר את התחום שבו אתה משתמש עבור אתר האינטרנט שלך ולאחר מכן בחר **הגדרות DNS** בחלונית הניהול.</span><span class="sxs-lookup"><span data-stu-id="5b471-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="5b471-104">בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5b471-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="5b471-105">עבור **סוג DNS** הזן: **A (כתובת)**</span><span class="sxs-lookup"><span data-stu-id="5b471-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="5b471-106">עבור **שם מארח או כינוי**, הקלד: **@**</span><span class="sxs-lookup"><span data-stu-id="5b471-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="5b471-107">עבור **כתובת IP**, הקלד את כתובת ה- IP הסטטית עבור אתר האינטרנט שלך במקום שבו הוא מתארח כעת (לדוגמה, 172.16.140.1‏).</span><span class="sxs-lookup"><span data-stu-id="5b471-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="5b471-p101">כתובת זו חייבת להיות כתובת IP  *סטטית*  עבור אתר האינטרנט, ולא כתובת IP  *דינאמית*  . בדוק באתר שבו מתארח אתר האינטרנט שלך כדי לוודא שבאפשרותך לקבל כתובת IP סטטית עבור אתר האינטרנט הציבורי.</span><span class="sxs-lookup"><span data-stu-id="5b471-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="5b471-110">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="5b471-110">Select **Save**.</span></span> 
    
<span data-ttu-id="5b471-111">ניתן גם ליצור רשומת CNAME כדי לעזור למבקרים למצוא את אתר האינטרנט שלך.</span><span class="sxs-lookup"><span data-stu-id="5b471-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="5b471-112">בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5b471-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="5b471-113">עבור **סוג DNS** הזן: **CNAME (כינוי)‎**</span><span class="sxs-lookup"><span data-stu-id="5b471-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="5b471-114">עבור **שם מארח או כינוי**, הקלד: **www**</span><span class="sxs-lookup"><span data-stu-id="5b471-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="5b471-115">עבור **כתובת מפנה**, הקלד את שם התחום המלא (FQDN) של אתר האינטרנט שלך (לדוגמה, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5b471-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="5b471-116">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="5b471-116">Select **Save**.</span></span> 
    

