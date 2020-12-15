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
# <a name="microsoft-edge-user-agent-string-desktop"></a>מחרוזת סוכן משתמשים של Microsoft Edge (שולחן העבודה)

ניתן להשתמש במחרוזות של סוכן משתמשים (UA) כדי לזהות איזו גירסה של דפדפן ספציפי נמצאת בשימוש במערכת הפעלה מסוימת. בדומה לדפדפנים אחרים, Microsoft Edge כולל מידע זה בכותרת HTTP של ' משתמש-סוכן ' בכל פעם שהוא מבצע בקשה לאתר. ניתן גם לגשת למידע בגירסת הדפדפן באמצעות JavaScript על-ידי שאילתת הערך של "navigator. userAgent".

אנו ממליצים על מפתחי אינטרנט לבצע שימוש בזיהוי תכונות כאשר ניתן לשפר את הקוד maintainability, לצמצם את שברירות הקוד, ולמנוע את הסיכון לניתוק קוד במקרה של עדכוני מחרוזת בעתיד של UA.

לקבלת מידע נוסף, ראה [מחרוזת סוכן משתמשים של Microsoft Edge (שולחן העבודה)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).