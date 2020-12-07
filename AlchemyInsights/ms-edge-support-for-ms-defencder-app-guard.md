---
title: התמיכה של microsoft Edge עבור המשמר היישומים של microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583583"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="e25fe-102">התמיכה של microsoft Edge עבור המשמר היישומים של microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="e25fe-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="e25fe-103">מיועד ל-Windows 10 ו-Microsoft Edge, מאבטח היישומים משתמש בגישה בידוד חומרה המאפשרת למשתמש לנווט באתר לא מהימן מתוך גורם מכיל מבודד, Hyper-V-זמין, כשהוא מופרד ממערכת ההפעלה המארחת.</span><span class="sxs-lookup"><span data-stu-id="e25fe-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="e25fe-104">מנהל ארגוני מגדיר רשימה של אתרי אינטרנט מהימנים, משאבי ענן ורשתות פנימיות.</span><span class="sxs-lookup"><span data-stu-id="e25fe-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="e25fe-105">כאשר משתמש מבקר באתר שאינו מכיל את הרשימה, Microsoft Edge יפתח את האתר בגורם המכיל.</span><span class="sxs-lookup"><span data-stu-id="e25fe-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="e25fe-106">משמעות הדבר היא שאם האתר יהפוך למזיק, המחשב המארח יישאר מוגן והתוקף לא יגיע לנתונים הארגוניים.</span><span class="sxs-lookup"><span data-stu-id="e25fe-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="e25fe-107">התקנת הרחבות בגורם המכיל נתמכת מכיוון Microsoft Edge גירסה 81, וניתן לשלוט בה באמצעות מדיניות.</span><span class="sxs-lookup"><span data-stu-id="e25fe-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="e25fe-108">יש להוסיף את כתובת updateURL הנמצאת בשימוש במדיניות ExtensionInstallForcelist כמשאב נייטרלי במדיניות בידוד הרשת המשמשת את משמר היישומים.</span><span class="sxs-lookup"><span data-stu-id="e25fe-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="e25fe-109">לקבלת מידע נוסף, ראה [תמיכה ב-Microsoft Edge עבור משמר היישומים של Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="e25fe-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
