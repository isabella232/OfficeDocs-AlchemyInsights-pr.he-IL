---
title: בעיה עם קבוצות אבטחה
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177495"
---
# <a name="issue-with-security-groups"></a>בעיה עם קבוצות אבטחה

**אם אתה מקבל את שגיאת הרשת AADDS104**

כללי קבוצת אבטחת רשת לא חוקיים הם הגורם הנפוץ ביותר לשגיאות רשת עבור שירותי התחום של תכלת Active Directory (AD DS). קבוצת אבטחת הרשת עבור הרשת הוירטואלית חייבת לאפשר גישה ליציאות ולפרוטוקולים ספציפיים. אם יציאות אלה נחסמות, לפלטפורמת התכלת אין אפשרות לנטר או לעדכן את התחום המנוהל. הסינכרון בין תכלת לספירה לבין תכלת AD DS מושפע אף הוא. ודא שאתה משאיר את יציאות ברירת המחדל פתוחות כדי למנוע הפרעה בשירות.

כדי להבין ולפתור התראות נפוצות עבור בעיות תצורה של קבוצת אבטחת רשת, ראה [הוספה ואימות של קבוצות אבטחה](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
