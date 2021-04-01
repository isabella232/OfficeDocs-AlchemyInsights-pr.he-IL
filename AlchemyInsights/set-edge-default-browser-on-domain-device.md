---
title: הגדרת Microsoft Edge כדפדפן ברירת המחדל במכשיר המצורף לתחום
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491585"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="706ce-102">הגדרת Microsoft Edge כדפדפן ברירת המחדל במכשיר המצורף לתחום</span><span class="sxs-lookup"><span data-stu-id="706ce-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="706ce-103">הגדר את Microsoft Edge כדפדפן ברירת המחדל:</span><span class="sxs-lookup"><span data-stu-id="706ce-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="706ce-104">[צור קובץ תצורה של שיוכי ברירת מחדל](https://go.microsoft.com/fwlink/?linkid=2132437) ולאחסן אותו באופן מקומי או משותף ברשת.</span><span class="sxs-lookup"><span data-stu-id="706ce-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="706ce-105">פתח את עורך המדיניות הקבוצתית ולאחר מכן עבור אל **תבניות**  >  **מנהליות של** תצורת מחשב סייר הקבצים של רכיבי  >    >  **Windows**.</span><span class="sxs-lookup"><span data-stu-id="706ce-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="706ce-106">בחר **הגדר קובץ תצורה של שיוכי ברירת מחדל.**</span><span class="sxs-lookup"><span data-stu-id="706ce-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="706ce-107">בחר **הגדרת מדיניות** ולאחר מכן בחר **זמין**.</span><span class="sxs-lookup"><span data-stu-id="706ce-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="706ce-108">תחת **אפשרויות**, הזן את המיקום של קובץ התצורה של שיוכי ברירת המחדל ולאחר מכן בחר **אישור.**</span><span class="sxs-lookup"><span data-stu-id="706ce-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
