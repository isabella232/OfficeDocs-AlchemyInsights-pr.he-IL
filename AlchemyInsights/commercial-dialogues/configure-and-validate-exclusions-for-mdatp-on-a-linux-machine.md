---
title: קביעת תצורה ואימות של פריטים מוכללים עבור MDATP במכונת לינוקס
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746023"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="764d0-102">קביעת תצורה ואימות של פריטים מוכללים עבור MDATP במכונת לינוקס</span><span class="sxs-lookup"><span data-stu-id="764d0-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="764d0-103">באפשרותך לכלול קבצים מסוימים, תיקיות, תהליכים וקבצים מסוימים שנפתחו בתהליך מסריקות MDATP.</span><span class="sxs-lookup"><span data-stu-id="764d0-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="764d0-104">אי-הכללה מסייעת למנוע זיהוי שגוי של תוכנות וקבצים באופן ייחודי או מותאם אישית לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="764d0-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="764d0-105">הוכללות גם מסייעות להקל על בעיות ביצועים שנגרמות על-ידי MDATP.</span><span class="sxs-lookup"><span data-stu-id="764d0-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="764d0-106">לקבלת מידע נוסף, ראה [קביעת תצורה ואימות של פריטים מוכללים עבור MDATP עבור Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="764d0-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="764d0-107">החריגים המתוארים במאמר זה אינם חלים על יכולות אחרות של MDATP עבור Linux, כולל זיהוי נקודות קצה ותגובה (EDR).</span><span class="sxs-lookup"><span data-stu-id="764d0-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="764d0-108">קבצים שאתה לא מכליל באמצעות השיטות המתוארות במאמר זה יכולים עדיין להפעיל התראות של EDR ויכולות זיהוי אחרות.</span><span class="sxs-lookup"><span data-stu-id="764d0-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
