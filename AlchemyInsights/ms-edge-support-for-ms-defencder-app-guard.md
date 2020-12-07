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
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>התמיכה של microsoft Edge עבור המשמר היישומים של microsoft Defender

מיועד ל-Windows 10 ו-Microsoft Edge, מאבטח היישומים משתמש בגישה בידוד חומרה המאפשרת למשתמש לנווט באתר לא מהימן מתוך גורם מכיל מבודד, Hyper-V-זמין, כשהוא מופרד ממערכת ההפעלה המארחת.

מנהל ארגוני מגדיר רשימה של אתרי אינטרנט מהימנים, משאבי ענן ורשתות פנימיות. כאשר משתמש מבקר באתר שאינו מכיל את הרשימה, Microsoft Edge יפתח את האתר בגורם המכיל. משמעות הדבר היא שאם האתר יהפוך למזיק, המחשב המארח יישאר מוגן והתוקף לא יגיע לנתונים הארגוניים.

התקנת הרחבות בגורם המכיל נתמכת מכיוון Microsoft Edge גירסה 81, וניתן לשלוט בה באמצעות מדיניות. יש להוסיף את כתובת updateURL הנמצאת בשימוש במדיניות ExtensionInstallForcelist כמשאב נייטרלי במדיניות בידוד הרשת המשמשת את משמר היישומים.

לקבלת מידע נוסף, ראה [תמיכה ב-Microsoft Edge עבור משמר היישומים של Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).
