---
title: אין אפשרות להגדיר או להציג את המדיניות ' אפשר שירותרכישה '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158562"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="39778-102">אין אפשרות להגדיר או להציג את המדיניות ' אפשר שירותרכישה '</span><span class="sxs-lookup"><span data-stu-id="39778-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="39778-103">בעת ניסיון להגדיר או להציג את המדיניות אפשר שירות הרכישה, מתקבלת הודעת השגיאה הבאה:</span><span class="sxs-lookup"><span data-stu-id="39778-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="39778-104">*שגיאת התקשרות: לא היתה אפשרות לאחזר מדיניות מוצר עם מזהה שירות ' אפשר שירותרכישה ', הודעת שגיאה-החיבור הבסיסי נסגר: אירעה שגיאה בלתי צפויה בשליחה.*</span><span class="sxs-lookup"><span data-stu-id="39778-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="39778-105">ייתכן שהסיבה לכך היא גירסה ישנה יותר של אבטחת שכבת התעבורה (TLS).</span><span class="sxs-lookup"><span data-stu-id="39778-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="39778-106">כדי לחבר את שירות MSCommerce, עליך להשתמש ב-TLS 1.2 או בגדול יותר.</span><span class="sxs-lookup"><span data-stu-id="39778-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="39778-107">נסה את השלבים הבאים כדי להפעיל/להגדיר את פרוטוקול TLS ל1.2, לאמת ולנסות שנית.</span><span class="sxs-lookup"><span data-stu-id="39778-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="39778-108">בשורת הפקודה PowerShell (PS C:\) הזן את הפקודה הבאה כדי להגדיר את פרוטוקול TLS לגירסה 1.2:</span><span class="sxs-lookup"><span data-stu-id="39778-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="39778-109">אמת את הפרוטוקולים של TLS בשימוש, עם הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="39778-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="39778-110">נסה שוב את הפקודות קבל או עדכן לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="39778-110">Retry the Get or Update commands as needed.</span></span>

