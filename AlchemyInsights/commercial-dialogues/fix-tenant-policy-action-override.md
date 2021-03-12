---
title: תיקון מדיניות דייר (עקיפת פעולה)
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
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745883"
---
# <a name="fix-tenant-policy-action-override"></a>תיקון מדיניות דייר (עקיפת פעולה)

מדיניות למניעת הודעות זבל בדייר שלך השפיעה על הודעה זו. כדי לסקור את המדיניות, בצע את הפעולות הבאות:

1. עבור אל [מרכז התאימות של & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)ולאחר מכן עבור אל מדיניות **ניהול האיום**  >    >  [נגד הודעות זבל](https://go.microsoft.com/fwlink/?linkid=2101518).
2. בדוק אם **מקור מדיניות** מציין את הפרטים הבאים:  **Add-Xheader/ModifySubject/ניתוב מחדש/מחיקה/אין הודעת פעולה/עותק מוסתר**

    אם כן, בכרטיסיה **התאמה אישית** , סמן את הגדרות המדיניות שהשפיעו על ההודעה. ייתכן **שההגדרות הרגילות** שהוחלו על כל לקוחות Exchange Online השפיעו על ההודעה.

לקבלת מידע נוסף אודות קביעת התצורה של פריטי מדיניות של מסנן דואר זבל, ראה [קביעת תצורה של מדיניות מסנן דואר הזבל](https://go.microsoft.com/fwlink/?linkid=2101431)
