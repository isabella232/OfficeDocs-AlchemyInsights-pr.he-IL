---
title: בקר תחום
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901024"
---
# <a name="domain-controller"></a>בקר תחום

**לא ניתן להפעיל את ה-עמ-DS או הפריסה נכשלים**

כדי לפתור את הבעיה של שירות התחומים של ' תכלת לספירה (עמ-DS) לא זמין או אם אינך מצליח לפרוס אותו, בצע את השלבים הבאים:

1. אם אתה משתמש ברשת וירטואלית קיימת כבר, סמן את NSG עבור כללים החוסמים את היציאות הדרושות כדי לסנכרן ב-עמ-DS בפורטל https://aka.ms/aadds-networking .
2. בדוק אם הודעת השגיאה שלך מתקבלת במדריך זה לפתרון בעיות שזמין ב  https://aka.ms/aadds-troubleshoot-enable -.
3. נסה לפרוס את שירותי התחומים של תכלת לספירה ברשת וירטואלית חדשה.
4. פעל לפי מדריך תחילת העבודה כיצד לפרוס את ה-DN-DS, הזמין [בערכת לימוד כדי ליצור שירותים בנושא תכלת AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. אם אתה נתקל בבעיות בפריסת שירותים מתחום שירותי התחומים, ראה [פתרון בעיות בנושא שירותי התחום של ' תכלת לספירה](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) ' כדי לפתור שגיאות נפוצות שיעזרו לך להפעיל שוב את העבודה. 

**לא ניתן להפוך את ה-עמ-DS ללא זמין**

לא ניתן להשהות את ה-עמ-DS. אם ברצונך להפסיק להשתמש בתחום המנוהל שלך, יש למחוק אותו.

אם אתה נתקל בבעיות, כדי לפתור הודעות שגיאה נפוצות ולגבי שלבי פתרון בעיות משויכים שיעזרו לך להפעיל שוב את העניינים, ראה [פתרון בעיות בשירותי התחום של Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
