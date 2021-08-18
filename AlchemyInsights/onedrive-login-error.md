---
title: OneDrive שגיאת כניסה AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112913"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive שגיאת כניסה AADSTS50011

אם אתה מקבל שגיאה "AADSTS50011: כתובת ה- URL של התשובה שצוינה בבקשה אינה תואמת לתשובה" בעת כניסה ליישום OneDrive, בדוק את הפעולות הבאות:

גירסת OneDrive שלך צריכה להיות שווה לגירסה 20.052.XXXX.XXXX.XXXX או גדולה יותר מגירסה 20.052.XXXX.XXXX. כדי לבדוק את הגירסה שלך, לחץ על סמל OneDrive הכחול באזור ההודעות, בחר **עזרה & הגדרות > הגדרות > אודות**.

הרשת שלך עשויה לחסום תעבורה **g.live.com ו-** **oneclient.sfx.ms**. אם תעבורה זו חסומה, אין OneDrive לעדכן את עצמה. עבוד עם מנהל הרשת כדי לוודא שיש לך גישה אל כתובות URL אלה. [נקודות קצה אלה אמורות](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) להיות נגישות עבור לקוחות המשתמשים Microsoft 365 תוכניות.

אם עליך לקבל באופן ידני גירסה נוכחית של OneDrive, בקר [https://aka.ms/getonedrive](https://aka.ms/getonedrive) ב- .
