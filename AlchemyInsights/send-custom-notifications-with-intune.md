---
title: שליחת הודעות מותאמות אישית באמצעות Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086165"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>כיצד לשלוח הודעות מותאמות אישית למשתמשים במכשירי iOS ו- Android מנוהלים

הודעות מותאמות אישית עבור Intune מעובדות Company Portal על-ידי אפליקציית המשתמש במכשיר של משתמש. לאחר מכן, האפליקציה יוצרת את הודעת דחיפה במכשיר זה.

להלן תנאים מוקדמים של מכשיר לתמיכה בקבלת הודעות מותאמות אישית, ולאחר מכן כדי שהיישום ייצור את הודעת דחיפה:

- המכשיר חייב להתקין את Company Portal היישום.  

- המכשיר חייב לאפשר לאפליקציה Company Portal לשלוח הודעות דחיפה. כאשר האפליקציה מותקנת או מתעדכנת, היא תבקש מהמשתמש להתיר הודעות.

- מכשירי Android חייבים להתקין את Google Play Services.

- המכשיר חייב להיות רשום באמצעות Intune.

לקבלת מידע נוסף, כולל אופן שליחת הודעה, עיין [בתיעוד התכונה](https://docs.microsoft.com/intune/custom-notifications).
