---
title: לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826092"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="5e417-102">לא ניתן להגדיר או להציג את מדיניות AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="5e417-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="5e417-103">בעת ניסיון להגדיר או להציג את מדיניות AllowSelfServicePurchase, מתקבלת הודעת השגיאה הבאה:</span><span class="sxs-lookup"><span data-stu-id="5e417-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="5e417-104">*HandleError : לא היתה אפשרות לאחזר מדיניות מוצר באמצעות PolicyId 'AllowSelfServicePurchase', ErrorMessage - החיבור שמשמש בסיס נסגר: אירעה שגיאה בלתי צפויה בשליחה.*</span><span class="sxs-lookup"><span data-stu-id="5e417-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="5e417-105">ייתכן שהגורם הוא גירסה קודמת של אבטחת שכבת תעבורה (TLS).</span><span class="sxs-lookup"><span data-stu-id="5e417-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="5e417-106">כדי לחבר את שירות MSCommerce, עליך להשתמש ב- TLS 1.2 לחלופין.</span><span class="sxs-lookup"><span data-stu-id="5e417-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="5e417-107">נסה את השלבים הבאים כדי להפעיל/להגדיר את פרוטוקול TLS ל- 1.2, לאמת ונסה שוב.</span><span class="sxs-lookup"><span data-stu-id="5e417-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="5e417-108">בשורת הפקודה של PowerShell (PS C: \) הזן את הפקודה הבאה כדי להגדיר את פרוטוקול TLS לגירסה 1.2:</span><span class="sxs-lookup"><span data-stu-id="5e417-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="5e417-109">אמת את הפרוטוקולים של TLS בשימוש, באמצעות הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="5e417-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="5e417-110">נסה שוב את הפקודות קבל או עדכן כצורך.</span><span class="sxs-lookup"><span data-stu-id="5e417-110">Retry the Get or Update commands as needed.</span></span>

