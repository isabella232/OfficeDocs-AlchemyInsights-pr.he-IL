---
title: מחרוזת סוכן משתמשים של Microsoft Edge (שולחן העבודה)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678098"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="99270-102">מחרוזת סוכן משתמשים של Microsoft Edge (שולחן העבודה)</span><span class="sxs-lookup"><span data-stu-id="99270-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="99270-103">ניתן להשתמש במחרוזות של סוכן משתמשים (UA) כדי לזהות איזו גירסה של דפדפן ספציפי נמצאת בשימוש במערכת הפעלה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="99270-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="99270-104">בדומה לדפדפנים אחרים, Microsoft Edge כולל מידע זה בכותרת HTTP של ' משתמש-סוכן ' בכל פעם שהוא מבצע בקשה לאתר.</span><span class="sxs-lookup"><span data-stu-id="99270-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="99270-105">ניתן גם לגשת למידע בגירסת הדפדפן באמצעות JavaScript על-ידי שאילתת הערך של "navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="99270-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="99270-106">אנו ממליצים על מפתחי אינטרנט לבצע שימוש בזיהוי תכונות כאשר ניתן לשפר את הקוד maintainability, לצמצם את שברירות הקוד, ולמנוע את הסיכון לניתוק קוד במקרה של עדכוני מחרוזת בעתיד של UA.</span><span class="sxs-lookup"><span data-stu-id="99270-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="99270-107">לקבלת מידע נוסף, ראה [מחרוזת סוכן משתמשים של Microsoft Edge (שולחן העבודה)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="99270-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>