---
title: שכפול הרשומה של המכשיר בפורטל
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814517"
---
# <a name="duplicate-device-record-in-the-portal"></a>שכפול הרשומה של המכשיר בפורטל

ייתכן שתראה 2 רשומות עבור מכשיר בפורטל אם המכשיר לא מדווח כראוי על מצב הניהול המשותף לאתר מנהל התצורה. כדי לבדוק את מצב הניהול המשותף של המכשיר, סקור את העמודה **'מנוהל במשותף'** עבור המכשיר במסוף מנהל התצורה. אם העמודה אינה גלויה, תוכל להוסיף אותה על-ידי לחיצה באמצעות לחצן העכבר הימני על כל אחת מכותרות העמודות ובחירתה מהרשימה.

הערך 'מנוהל במשותף' חייב להיות **'כן'**. אם הערך הוא **'לא'**, פתח את יישומון הלקוח של מנהל התצורה במכשיר הלקוח ובדוק את המאפיין **'ניהול משותף'** בכרטיסיה כללי.

- אם הערך הוא **'זמין'**, משמעות הדבר היא בעיות בתקשורת לקוח עם נקודת הניהול. עיין ב **CcmMessaging.log** במכשיר כדי לחקור בעיות קישוריות פוטנציאליות.

- אם הערך הוא **'לא זמין'** והמכשיר רשום באמצעות Intune, ודא שהמכשיר קיבל מדיניות ניהול משותף על-ידי סקירת **CoManagementHandler.log** במכשיר.
