---
title: לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735200"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="75cdc-102">לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="75cdc-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="75cdc-103">בעת ניסיון להגדיר או להציג את מדיניות AllowSelfServicePurchase, אתה מקבל את הודעת השגיאה הבאה:</span><span class="sxs-lookup"><span data-stu-id="75cdc-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="75cdc-104">*HandleError: לא היתה אפשרות לאחזר מדיניות מוצר עם PolicyId ' AllowSelfServicePurchase ', ErrorMessage-החיבור המשמש כבסיס נסגר: אירעה שגיאה בלתי צפויה בשליחה.*</span><span class="sxs-lookup"><span data-stu-id="75cdc-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="75cdc-105">ייתכן שהסיבה לכך היא גירסה ישנה יותר של אבטחה בשכבת התעבורה (TLS).</span><span class="sxs-lookup"><span data-stu-id="75cdc-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="75cdc-106">כדי לחבר את שירות MSCommerce, עליך להשתמש ב-TLS 1.2 או בגדול יותר.</span><span class="sxs-lookup"><span data-stu-id="75cdc-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="75cdc-107">נסה את השלבים הבאים כדי להפעיל/להגדיר את פרוטוקול TLS ל-1.2, לאמת ולנסות שוב.</span><span class="sxs-lookup"><span data-stu-id="75cdc-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="75cdc-108">בשורת הפקודה של PowerShell (PS C: \) הזן את הפקודה הבאה כדי להגדיר את הפרוטוקול TLS לגירסה 1.2:</span><span class="sxs-lookup"><span data-stu-id="75cdc-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="75cdc-109">ודא שהפרוטוקולים של TLS נמצאים בשימוש, באמצעות הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="75cdc-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="75cdc-110">נסה שוב לבצע את הפקודות קבל או עדכן לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="75cdc-110">Retry the Get or Update commands as needed.</span></span>

