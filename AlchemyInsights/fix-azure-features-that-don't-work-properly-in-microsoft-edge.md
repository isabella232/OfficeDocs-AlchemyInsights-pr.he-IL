---
title: מה לעשות אם תכונות התכלת אינם פועלים כראוי ב-Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583461"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="4f9e4-102">מה לעשות אם תכונות התכלת אינם פועלים כראוי ב-Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4f9e4-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="4f9e4-103">ל-Microsoft Edge יש [בעיות ידועות](https://go.microsoft.com/fwlink/?linkid=2140608) הקשורות לאזורי אבטחה ועשויות להשפיע על האופן שבו משתמשי התכלת נכנסו למרכז הניהול של Windows.</span><span class="sxs-lookup"><span data-stu-id="4f9e4-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="4f9e4-104">אם אתה נתקל בבעיות בשימוש בתכונות תכלת עם Microsoft Edge, נסה את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="4f9e4-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="4f9e4-105">בתפריט **התחל** , חפש את **אפשרויות האינטרנט** ובחר אותה.</span><span class="sxs-lookup"><span data-stu-id="4f9e4-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="4f9e4-106">בתיבת הדו **מאפייני אינטרנט** , עבור אל הכרטיסיה **אבטחה** .</span><span class="sxs-lookup"><span data-stu-id="4f9e4-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="4f9e4-107">בחר את אזור **האתרים המהימנים** ולאחר מכן בחר בלחצן **אתרים** .</span><span class="sxs-lookup"><span data-stu-id="4f9e4-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="4f9e4-108">בתיבת הדו **אתרים מהימנים** , הוסף את כתובת ה-URL של השער וכן הלאה [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) ולאחר מכן בחר **סגור**.</span><span class="sxs-lookup"><span data-stu-id="4f9e4-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="4f9e4-109">בתיבת הדו **מאפייני אינטרנט** , עבור אל הכרטיסיה **פרטיות** .</span><span class="sxs-lookup"><span data-stu-id="4f9e4-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="4f9e4-110">במקטע **חוסם הפריטים המוקפצים** , בחר באפשרות **הגדרות**.</span><span class="sxs-lookup"><span data-stu-id="4f9e4-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="4f9e4-111">בתיבת הדו שנפתחת, הוסף את כתובת ה-URL של השער וכן הלאה [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) ולאחר מכן בחר **סגור**.</span><span class="sxs-lookup"><span data-stu-id="4f9e4-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
