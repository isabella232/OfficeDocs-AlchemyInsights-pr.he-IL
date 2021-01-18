---
title: קביעת תצורה של שירות תחום
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885222"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>לא ניתן להפעיל את ה-עמ-DS או הפריסה נכשלים

כדי לפתור את הבעיה של שירות התחומים של ' תכלת לספירה (עמ-DS) לא זמין או אם אינך מצליח לפרוס אותו, בצע את השלבים הבאים:

1. אם אתה משתמש ברשת וירטואלית קיימת כבר, סמן את NSG עבור כללים החוסמים את היציאות הדרושות כדי לסנכרן ב-עמ-DS בפורטל https://aka.ms/aadds-networking .
2. בדוק אם הודעת השגיאה שלך מתקבלת במדריך זה לפתרון בעיות שזמין ב  https://aka.ms/aadds-troubleshoot-enable -.
3. נסה לפרוס את שירותי התחומים של תכלת לספירה ברשת וירטואלית חדשה.
4. פעל לפי מדריך תחילת העבודה כיצד לפרוס את ה-DN-DS: [צור וקבע את התצורה של שירותי תחומים](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)של dn.
5. אם אתה נתקל בבעיות בפריסת שירותים מתחום שירותי התחומים, ראה [פתרון בעיות בנושא שירותי התחום של ' תכלת לספירה](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) ' כדי לפתור שגיאות נפוצות שיעזרו לך להפעיל שוב את העבודה. 

**לא ניתן להפוך את ה-עמ-DS ללא זמין**

לא ניתן להשהות את ה-עמ-DS. אם ברצונך להפסיק להשתמש בתחום המנוהל שלך, יש למחוק אותו.
כדי למחוק את התחום המנוהל שלך, ראה [מחיקת שירות תחומים בתחום](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



