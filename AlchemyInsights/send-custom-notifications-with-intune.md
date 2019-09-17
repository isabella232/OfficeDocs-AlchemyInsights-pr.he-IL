---
title: שליחת הודעות מותאמות אישית עם Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992314"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>כיצד לשלוח הודעות מותאמות אישית למשתמשי iOS מנוהלים והתקנים אנדרואיד

הודעות מותאמות אישית עבור Intune מעובדות על-ידי יישום פורטל החברה בהתקן של משתמש. לאחר מכן, האפליקציה יוצרת את הודעת הדחיפה על המכשיר.

להלן דרישות מוקדמות של התקנים כדי לתמוך בקבלת הודעות מותאמות אישית, ועבור היישום לאחר מכן ליצור את הודעת הדחיפה:

- ההתקן חייב להתקין את יישום הפורטל של החברה.  

- ההתקן חייב לאפשר ליישום פורטל החברה לשלוח הודעות דחיפה. כאשר האפליקציה מותקנת או מתעדכנת, היא תנחה את המשתמש להתיר הודעות.

- התקנים אנדרואיד חייב להיות Google Play שירותי מותקן.

- המכשיר חייב להיות רשום עם Intune.

לקבלת מידע נוסף כולל כיצד לשלוח הודעה, עיין [בתיעוד של התכונה](https://docs.microsoft.com/intune/custom-notifications).
