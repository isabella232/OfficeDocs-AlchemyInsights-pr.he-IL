---
title: תיקון מדיניות חיבור
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694166"
---
# <a name="fix-connection-policy"></a>תיקון מדיניות חיבור

הודעת הדואר האלקטרוני סומנה כבטוחה ונמסרה לתיבת הדואר הנכנס של המשתמש מאחר שכתובת ה-IP השולחת סומנה כבטוחה במדיניות מסנן החיבורים. כדי לסקור את המדיניות, בצע את הפעולות הבאות:

1. עבור אל [מרכז התאימות של & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)ולאחר מכן עבור אל מדיניות **ניהול האיום**  >    >  [נגד הודעות זבל](https://go.microsoft.com/fwlink/?linkid=2101518).
2. בכרטיסיה **התאמה אישית** , בחר את **מדיניות מסנן החיבורים** ולאחר מכן בחר **ערוך מדיניות**.
3. סקור את רשימת **ההיתרים של IP** . ראה אם **הרשימה הבטוחה** מאופשרת.

    > [!NOTE]
    > Microsoft נרשמת כמנוי למקורות ספקים חיצוניים של שולחים מהימנים. אם **הרשימה הבטוחה** מופעלת, שולחים מהימנים אלה לא מסומנים בטעות כדואר זבל. אני ממליץ לבחור באפשרות זו, משום שהיא תקטין את מספר החיובים החיוביים הכוזבים (דואר טוב שמסווג כדואר זבל) שאתה מקבל.
