---
title: לא נמצאו הודעות של מנויים במרכז האבטחה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544109"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>לא נמצאו הודעות של מנויים במרכז האבטחה

אם בעת הגישה מרכז האבטחה של Microsoft Defender אתה מקבל הודעת "לא נמצאו מנויים", פירוש הדבר ש- Azure Active Directory (AAD) המשמש כדי להיכנס למשתמש לפורטל אינו כולל רשיון Microsoft Defender ATP.  

הרשיונות Windows E5 Office E5 הם רשיונות נפרדים.

פתח מקרה תמיכה אם הרשיון נרכש אך לא הוקצה למופע AAD זה. או שיש לך: <br/>
-   בעיה אפשרית בהקצאת רשיון.<br/>
-   הקצאת בטעות את הרשיון ל- AAD אחר של Microsoft מזה ששימש לאימות בשירות.