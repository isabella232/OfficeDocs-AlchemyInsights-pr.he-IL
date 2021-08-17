---
title: העברה אוטומטית של הודעות דואר אלקטרוני לתיבת הדואר של הארכיון
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059227"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>העברה אוטומטית של הודעות דואר אלקטרוני לתיבת הדואר של הארכיון

כך ניתן להגדיר מדיניות כדי להעביר באופן אוטומטי דואר אלקטרוני ישן של משתמש לתיבת הדואר של הארכיון:

1. עבור אל [**ארכיון &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **פיקוח על** נתוני  >  **תאימות** כדי לוודא שתיבת דואר של ארכיון זמינה עבור המשתמש. אם לא, לחץ על **הפוך לזמין** ולאחר **מכן על כן** בתיבת האזהרה.
2. עבור אל [**Exchange הניהול של > תאימות > תגיות שמירה**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. בחר את סמל + ולאחר מכן בחר **החל באופן אוטומטי על תיבת הדואר כולה**.
4. הקצה שם לתג השמירה ובחר העבר **לארכיון**. עבור תקופת השמירה, הזן את השעה הרצויה, כגון 90 יום. לחץ על **שמור**.
5. כעת צור מדיניות שמירה: בחר **מדיניות שמירה,** בחר את הסמל כדי להוסיף מדיניות חדשה.
6. הקצה שם למדיניות השמירה ולאחר מכן לחץ וגלול כדי לחפש ולהוסיף את תגית השמירה שיצרת זה עתה. לחץ על **שמור**.
7. לבסוף, החל את מדיניות השמירה על תיבת הדואר של המשתמש: עדיין במרכז Exchange, עבור אל **תיבות דואר**  >  **של נמענים**. בחר את כל המשתמשים שברצונך להחיל את המדיניות שלהם ולאחר מכן בחר **ערוך** (סמל העיפרון).
8. בתיבת הדו-שיח, לחץ על **תכונות תיבת דואר**. תחת **מדיניות שמירה**, החל את המדיניות שיצרת זה עתה > **שמור**.
9. לקבלת הוראות להחלת המדיניות על כל המשתמשים, ראה [החלת מדיניות שמירה על תיבות דואר.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
