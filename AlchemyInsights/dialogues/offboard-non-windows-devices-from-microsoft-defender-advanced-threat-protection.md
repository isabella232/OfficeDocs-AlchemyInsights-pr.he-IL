---
title: Offboard מכשירים שאינם של Windows מהגנת האיום המתקדמים של Microsoft Defender (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693814"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="13f83-102">Offboard מכשירים שאינם של Windows מהגנת האיום המתקדמים של Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="13f83-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="13f83-103">כך ניתן לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="13f83-103">Here's how:</span></span>

1. <span data-ttu-id="13f83-104">פעל בהתאם לתיעוד של הצד השלישי לניתוק הפתרון של ספק חיצוני מ-Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="13f83-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="13f83-105">מתוך דייר ה-Active Directory שלך, הסר הרשאות עבור הפתרון של ספק חיצוני:</span><span class="sxs-lookup"><span data-stu-id="13f83-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="13f83-106">היכנס [לפורטל התכלת](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="13f83-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="13f83-107">בחר **את כל השירותים**  >  **המפעילים** את  >  **היישומים הארגוניים** של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="13f83-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="13f83-108">בחר את היישום שברצונך לoffboard.</span><span class="sxs-lookup"><span data-stu-id="13f83-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="13f83-109">בחר **מחק**.</span><span class="sxs-lookup"><span data-stu-id="13f83-109">Select **Delete**.</span></span>

<span data-ttu-id="13f83-110">לקבלת מידע נוסף, ראה [Offboard מכשירים שאינם של Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="13f83-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
