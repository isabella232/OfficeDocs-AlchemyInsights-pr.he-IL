---
title: פתרון בעיות בהתקנת MDATP ב-Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746303"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="b57ae-102">פתרון בעיות בהתקנת MDATP ב-Mac</span><span class="sxs-lookup"><span data-stu-id="b57ae-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="b57ae-103">אם ההתקנה הידנית נכשלת, דף **הסיכום** של אשף ההתקנה מציג את השגיאה הבאה:</span><span class="sxs-lookup"><span data-stu-id="b57ae-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="b57ae-104">"אירעה שגיאה במהלך ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="b57ae-104">"An error occurred during installation.</span></span> <span data-ttu-id="b57ae-105">תוכנית ההתקנה נתקלה בשגיאה שגרמה להתקנה להיכשל.</span><span class="sxs-lookup"><span data-stu-id="b57ae-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="b57ae-106">פנה ליצרן התוכנה לקבלת סיוע.</span><span class="sxs-lookup"><span data-stu-id="b57ae-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="b57ae-107">עבור פריסות MDM, הדף מציג כשל כללי בהתקנה.</span><span class="sxs-lookup"><span data-stu-id="b57ae-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="b57ae-108">למרות שאין באפשרותנו להציג שגיאות מדויקות למשתמשי הקצה, אנו שועטים את קובץ יומן הרישום עם התקדמות ההתקנה, ב- **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="b57ae-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="b57ae-109">כל הפעלת התקנה מצורפת לקובץ יומן רישום זה.</span><span class="sxs-lookup"><span data-stu-id="b57ae-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="b57ae-110">כדי להפיק פלט של הפעלת ההתקנה האחרונה בלבד, השתמש באפשרות `sed` .</span><span class="sxs-lookup"><span data-stu-id="b57ae-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="b57ae-111">לקבלת מידע נוסף, ראה [פתרון בעיות התקנה עבור Microsoft DEFENDER ATP עבור Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="b57ae-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
