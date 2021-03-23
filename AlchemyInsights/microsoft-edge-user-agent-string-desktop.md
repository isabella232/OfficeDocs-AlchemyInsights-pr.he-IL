---
title: מחרוזות סוכן משתמשים של Microsoft Edge (שולחן עבודה)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8221"
- "9004596"
ms.openlocfilehash: 42c39f5661f57c7b57fa471f9c204e5c27f2f214
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036153"
---
# <a name="microsoft-edge-user-agent-strings-desktop"></a><span data-ttu-id="d7f0c-102">מחרוזות סוכן משתמשים של Microsoft Edge (שולחן עבודה)</span><span class="sxs-lookup"><span data-stu-id="d7f0c-102">Microsoft Edge user agent strings (Desktop)</span></span>

<span data-ttu-id="d7f0c-103">ניתן להשתמש במחרוזות של סוכן משתמשים (UA) כדי לזהות איזו גירסה של דפדפן ספציפי נמצאת בשימוש במערכת הפעלה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="d7f0c-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="d7f0c-104">בדומה לדפדפנים אחרים, Microsoft Edge כולל מידע זה בכותרת HTTP של ' משתמש-סוכן ' בכל פעם שהוא מבצע בקשה לאתר.</span><span class="sxs-lookup"><span data-stu-id="d7f0c-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="d7f0c-105">ניתן גם לגשת אליו באמצעות JavaScript על-ידי שאילתה על הערך של "navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="d7f0c-105">It can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="d7f0c-106">אנו ממליצים על מפתחי אינטרנט לבצע שימוש בזיהוי תכונות כאשר ניתן לשפר את הקוד maintainability, לצמצם את שברירות הקוד, ולמנוע את הסיכון לניתוק קוד במקרה של עדכוני מחרוזת בעתיד של UA.</span><span class="sxs-lookup"><span data-stu-id="d7f0c-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="d7f0c-107">לקבלת מידע נוסף, ראה [מחרוזת סוכן משתמשים של Microsoft Edge (שולחן העבודה)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="d7f0c-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>

