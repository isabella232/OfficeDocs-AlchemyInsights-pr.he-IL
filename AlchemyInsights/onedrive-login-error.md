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
# <a name="onedrive-login-error-aadsts50011"></a>שגיאת כניסה של OneDrive AADSTS50011

אם אתה מקבל שגיאה "AADSTS50011: כתובת ה-URL של התשובה שצוינה בבקשה אינה תואמת לתשובה" בעת הכניסה לאפליקציית OneDrive, בדוק את הפרטים הבאים:

גירסת OneDrive צריכה להיות שווה ל-or גדול מ-version 20.052. XXXX. XXXX. כדי לבדוק את הגירסה שלך, לחץ על סמל OneDrive הכחול באזור ההודעות, בחר **עזרה & הגדרות > הגדרות >**.

הרשת שלך עשויה לחסום תעבורה אל **g.live.com** ו- **oneclient.sfx.ms**. אם תעבורה זו חסומה, ל-OneDrive אין אפשרות לעדכן את עצמו. עבוד עם מנהל הרשת כדי לוודא שיש לך גישה לכתובות Url אלה. [נקודות קצה אלה](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) אמורות להיות נגישות עבור לקוחות המשתמשים בתוכניות Microsoft 365.

אם עליך לקבל באופן ידני גירסה נוכחית של OneDrive, בקר באתר [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
