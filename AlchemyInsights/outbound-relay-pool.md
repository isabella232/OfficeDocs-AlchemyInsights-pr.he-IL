---
title: מאגר ממסר יוצא
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041587"
---
# <a name="outbound-relay-pool"></a>מאגר ממסר יוצא

Microsoft גורמת לשינויים מסוימים בתצורה עבור העברה או העברה של דואר אלקטרוני באמצעות Microsoft 365. הודעות בתרחישים מסוימים מועברות או מועברות דרך Microsoft 365 באמצעות מאגר ממסר מיוחד. הודעות הנשלחות באמצעות מאגר הממסר עלולות להסתיים בתיקיית דואר הזבל של הנמען. לקבלת מידע נוסף, ראה [מקורות מסירה יוצאים](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

כדי להימנע מתרחיש באמצעות מאגר הממסר, ודא שהודעות שהועברו/ממסר יפגשו באחד מהקריטריונים הבאים:

- השולח היוצא הוא תחום מקובל של הדייר.
- Sender Policy Framework (SPF) עובר כאשר ההודעה מגיעה Microsoft 365.
- DomainKeys Identified Mail (DKIM) בתחום שולח P2 עובר כאשר ההודעה מגיעה Microsoft 365.
 
הודעות המנוהות לקריטריונים לעיל הבאות לא יעבירו דרך מאגר הממסרים.

אם רשומת ה- MX עבור התחום שלך מופנה לשרת של ספקים אחרים או לשרת מקומי, השתמש בסינון משופר כדי לוודא שאימות ה- SPF נכון עבור דואר אלקטרוני נכנס ולהימנע משליחה של דואר אלקטרוני דרך מאגר הממסרים.

**כיצד נוכל לדעת אם מאגר הממסר משפיע עלינו?**

אם הודעות הדואר האלקטרוני שהועברו או מועברות משתמשות באחד מהקריטריונים לעיל, הודעות לא ימסרו דרך מאגר הממסרים. עם זאת, אם הודעה נשלחת דרך מאגר ממסר, ה- IP של השרת היוצא נמצא בטווח 40.95.0.0/16, שם השרת היוצא כולל **rly** בשם.

