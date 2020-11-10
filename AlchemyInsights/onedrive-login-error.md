---
title: שגיאת כניסה של OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982479"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="403e9-102">שגיאת כניסה של OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="403e9-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="403e9-103">אם אתה מקבל שגיאה "AADSTS50011: כתובת ה-URL של התשובה שצוינה בבקשה אינה תואמת לתשובה" בעת הכניסה לאפליקציית OneDrive, בדוק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="403e9-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="403e9-104">גירסת OneDrive צריכה להיות שווה ל-or גדול מ-version 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="403e9-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="403e9-105">כדי לבדוק את הגירסה שלך, לחץ על סמל OneDrive הכחול באזור ההודעות, בחר **עזרה & הגדרות > הגדרות >**.</span><span class="sxs-lookup"><span data-stu-id="403e9-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="403e9-106">הרשת שלך עשויה לחסום תעבורה אל **g.live.com** ו- **oneclient.sfx.ms**.</span><span class="sxs-lookup"><span data-stu-id="403e9-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="403e9-107">אם תעבורה זו חסומה, ל-OneDrive אין אפשרות לעדכן את עצמו.</span><span class="sxs-lookup"><span data-stu-id="403e9-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="403e9-108">עבוד עם מנהל הרשת כדי לוודא שיש לך גישה לכתובות Url אלה.</span><span class="sxs-lookup"><span data-stu-id="403e9-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="403e9-109">[נקודות קצה אלה](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) אמורות להיות נגישות עבור לקוחות המשתמשים בתוכניות Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="403e9-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="403e9-110">אם עליך לקבל באופן ידני גירסה נוכחית של OneDrive, בקר באתר [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="403e9-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
