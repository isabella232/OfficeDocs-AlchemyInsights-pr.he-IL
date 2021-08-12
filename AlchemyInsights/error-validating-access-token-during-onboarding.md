---
title: אירעה שגיאה בעת אימות שגיאת אסימון גישה במהלך ניתוח שולחן העבודה בעת העלייה למטוס
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946616"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>שגיאת "אירעה שגיאה בעת אימות אסימון גישה" במהלך ההסתה ל- Desktop Analytics

שגיאה זו נצפתה בדרך כלל כאשר פג תוקפו של אסימון האימות. בדרך כלל, רענון הדף מרענן את האסימון. עם זאת, בעיה זו עשויה לפתור אם חלה מדיניות Access מותנית כלשהי שחלה על החשבון המשמש לניתוח שולחני על הלוח. באפשרותך לסקור את יומני הרישום של Azure AD Sign In בפורטל Azure כדי לראות אם זמינים כשלים בכניסה עבור החשבון המשמש עבור הכניסה ל- Desktop Analytics.

לקבלת מידע נוסף אודות תות Access, בקר ב [תכנון פריסת Access מותן](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).