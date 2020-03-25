---
title: לא ניתן להיכנס לצוותים עקב שגיאה autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932044"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>לא ניתן להיכנס לצוותים עקב שגיאה autologon.microsoftazuread-sso dot com:443

אם האפשרות Seamless SSO זמינה כאימות O365, ייתכן שיהיה צורך להוסיף את כתובת ה- URL "autologon.microsoftazuread-sso.com" לאתרי אינטרא-נט.  אם היא נוספה בעבר לאתרים מהימנים ו-Seamless SSO נמצאת בשימוש, יש להסיר אותה מאתרים מהימנים.

עיין ב- [רשימת פעולות לביצוע של פתרון בעיות ב-Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

בצע שלבים אלה כדי להוסיף כתובת URL לרשימה 'אתרי אינטרא-נט':

1. פתח את Internet Explorer על-ידי לחיצה על לחצן **התחל**. בתיבת החיפוש, הקלד Internet Explorer ולאחר מכן, ברשימת התוצאות, לחץ על **Internet Explorer**.
2. לחץ על **כלים** ולאחר מכן לחץ על **אפשרויות אינטרנט**.
3. לחץ על הכרטיסיה **אבטחה**.
4. כעת לחץ על **אתרי אינטרא-נט מקומיים** ולאחר מכן לחץ על הלחצן **אתרים** ולאחר מכן על הלחץ **מתקדם**.
5. הזן את כתובת ה-URL של אתר האינטרנט ולחץ על **הוסף**.
6. כשתסיים, לחץ על **סגור**.

לקבלת מידע נוסף, ראה [תיעוד עבור פריסת Seamless SSO עבור O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (כולל תהליך מבוסס על מדיניות כדי להוסיף כתובת URL אל אתרי אינטרנט בשלב 3).
