---
title: סינכרון hash של סיסמאות עבור שירות תחום
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177490"
---
# <a name="password-hash-synchronization-for-domain-service"></a>סינכרון hash של סיסמאות עבור שירות תחום

**אם המופע של ' תכלת AD DS ' מציג בקשה להפיכת סינכרון hash של סיסמאות לזמין**

אתה נתקל בתרחיש שבו אתה מפעיל סביבה היברידית שבה משתמשים מתנגדים מסביבה מקומית של תכלת Active Directory Domain Services (AD DS). תרחיש זה מתקיים למרות שאתה נתקל בסינכרון hash של סיסמאות מתוך AD DS המקומי לדייר המודע של תכלת.

**גורם**

פעולה זו מתבצעת מכיוון ש-תכלת AD Connect כברירת מחדל אינו מסנכרן רכיבי hash של מנהל LAN חדש מדור קודם (NTLM) ו-Kerberos הדרושים עבור ' תכלת AD DS '.

**פתרון** 

יהיה עליך לקבוע את התצורה של התחברות מסוג תכלת AD כדי לסנכרן קודי hash אלה הדרושים עבור אימות NTLM ו-Kerberos.

לאחר קביעת התצורה של התחברות מודעות מיידיות, האירוע ' יצירת חשבון מקומי ' או ' שינוי סיסמה ' מסנכרן גם את קודי ה-hash של הסיסמה המורשית לכיוון תכלת לספירה. ראה [כאן](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) לקבלת מידע נוסף על כך ולקבלת הנחיות להפיכת סינכרון סיסמאות לזמין בסביבות היברידית של תכלת AD DS.