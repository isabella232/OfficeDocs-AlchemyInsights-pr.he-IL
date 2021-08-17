---
title: יצירת הודעת דואר אלקטרוני תופסת הכל
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080747"
---
# <a name="create-an-email-catch-all"></a>יצירת הודעת דואר אלקטרוני תופסת הכל

השימוש במלכוד אינו מיואש במיוחד. עדיף לספק קפיצה חזרה לשולח, כך ששולחים יודעים שלא היתה אפשרות להעביר את ההודעה שלהם ככתובת כך שהם יכולים לבצע פעולה. באפשרותך גם להגביל את תיבת הדואר המנוהלת כדי לתפוס רק כתובות דואר אלקטרוני חוקיות בעבר. 

כל תפיסה של כל תיבת הדואר תקבל עסקה טובה של דואר זבל, ובסופו של דבר עשויה למלא אותה אם לא תנטר אותה מקרוב. (ישנם מגבלות קבלה.) 

אם תחליט להמשיך, בצע את השלבים הבאים:

1. יצירת קבוצת תפוצה דינאמית & "כל סוגי הנמענים".

2. צור תיבת דואר ייעודית כדי לתפוס הודעות דואר אלקטרוני, לדוגמה, catchall@domain.com.

3. עבור התחום הספציפי, הגדר את DomainType ל- "InternalRelay". אם תסיר מאוחר יותר את התלכוד הכל, הקפד להגדיר את התחום בחזרה ל'סמכותי'.

4. צור כלל תעבורה של זרימת דואר באופן הבא:

    - אם השולח הוא "מחוץ לארגון"
    - ניתוב מחדש של ההודעה Catchall@domain.com
    - למעט אם הנמען חבר ב- allusers@domain.com (קבוצת תפוצה מכילה את כל החברים)
    - ודא כי תיבות דואר חדשות מתווספות לקבוצת התפוצה הדינאמית
