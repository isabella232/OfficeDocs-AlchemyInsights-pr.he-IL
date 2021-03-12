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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746042"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>העברה אוטומטית של הודעות דואר אלקטרוני לתיבת הדואר של הארכיון

כך ניתן להגדיר מדיניות כדי להעביר באופן אוטומטי את הדואר האלקטרוני הישן של המשתמש לתיבת הדואר של הארכיון:

1. עבור אל [**ארכיון אבטחה & תאימות**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  '**ממשל נתונים**  >   ' כדי לוודא שתיבת דואר של ארכיון הופעלה עבור המשתמש. אם לא, לחץ על **הפוך לזמין** **בתיבת** האזהרה.
2. עבור אל [**מרכז הניהול של Exchange > ניהול תאימות > תגיות שמירה**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. בחר את סמל + ולאחר מכן בחר **החל באופן אוטומטי על תיבת הדואר כולה**.
4. הקצה שם לתגית השמירה ובחר **העבר לארכיון**. עבור תקופת השמירה, הזן את השעה הרצויה, כגון 90 ימים. לחץ על **שמור**.
5. כעת צור מדיניות שמירה: בחר באפשרות מדיניות **שמירה**, בחר את הסמל כדי להוסיף מדיניות חדשה.
6. הקצה שם למדיניות השמירה ולאחר מכן לחץ וגלול כדי לחפש ולהוסיף את תג השמירה שיצרת זה עתה. לחץ על **שמור**.
7. לבסוף, החל את מדיניות השמירה על תיבת הדואר של המשתמש: עדיין במרכז הניהול של Exchange, עבור אל  >  **תיבות הדואר** של הנמענים. בחר את כל המשתמשים שברצונך להחיל עליהם את המדיניות ולאחר מכן בחר **Edit** (סמל העיפרון).
8. בתיבת הדו, לחץ על **תכונות תיבת דואר**. תחת **מדיניות שמירה**, החל את המדיניות שיצרת זה עתה > **שמירה**.
9. לקבלת הוראות להחלת המדיניות על כל המשתמשים, ראה [החלת מדיניות שמירה על תיבות דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
