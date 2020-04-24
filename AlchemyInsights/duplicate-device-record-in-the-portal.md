---
title: שכפול הרשומה של המכשיר בפורטל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789863"
---
# <a name="duplicate-device-record-in-the-portal"></a>שכפול הרשומה של המכשיר בפורטל

ייתכן שתראה 2 רשומות עבור מכשיר בפורטל אם המכשיר לא מדווח כראוי על מצב הניהול המשותף לאתר מנהל התצורה. כדי לבדוק את מצב הניהול המשותף של המכשיר, סקור את העמודה **'מנוהל במשותף'** עבור המכשיר במסוף מנהל התצורה. אם העמודה אינה גלויה, תוכל להוסיף אותה על-ידי לחיצה באמצעות לחצן העכבר הימני על כל אחת מכותרות העמודות ובחירתה מהרשימה.

הערך 'מנוהל במשותף' חייב להיות **'כן'**. אם הערך הוא **'לא'**, פתח את יישומון הלקוח של מנהל התצורה במכשיר הלקוח ובדוק את המאפיין **'ניהול משותף'** בכרטיסיה כללי.

- אם הערך הוא **'זמין'**, משמעות הדבר היא בעיות בתקשורת לקוח עם נקודת הניהול. עיין ב **CcmMessaging.log** במכשיר כדי לחקור בעיות קישוריות פוטנציאליות.

- אם הערך הוא **'לא זמין'** והמכשיר רשום באמצעות Intune, ודא שהמכשיר קיבל מדיניות ניהול משותף על-ידי סקירת **CoManagementHandler.log** במכשיר.
