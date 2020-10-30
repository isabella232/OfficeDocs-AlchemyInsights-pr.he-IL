---
title: סוגי מנויים נתמכים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807563"
---
# <a name="supported-subscription-types"></a>סוגי מנויים נתמכים

עיין בסוגי המנויים הנתמכים כדי להמשיך עוד.

[סוגי מנויים נתמכים](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**העברת בעלות על חיוב**

הפורטל ' תכלת ' [כמנהל החשבון](https://ms.portal.azure.com/) של חשבון החיוב הכולל את המנוי שברצונך להעביר

- חיפוש **בניהול עלויות + חיוב** . בחר **מנויים** מחלונית שמאלית. בהתאם לגישה, ייתכן שיהיה עליך לבחור טווח חיוב ולאחר **מכן להיכנס** למנויים או **למנויי תכלת** .
- בחר העבר בעלות על חיוב עבור המנוי שברצונך להעביר
- הזן את כתובת הדואר האלקטרוני של משתמש שהוא מנהל חיוב של החשבון שיהיה הבעלים החדש עבור המנוי ולאחר מכן בחר **שלח בקשת העברה**
- המשתמש יקבל דואר אלקטרוני עם הוראות לסקירת בקשת ההעברה. כדי לאשר את בקשת ההעברה, המשתמש בוחר את הקישור בהודעת הדואר האלקטרוני ועוקב אחר ההוראות.

הערה: אם אתה מעביר את בעלות החיוב של המנוי שלך לחשבון של משתמש בדייר אחר של תכלת לספירה, כל הקצאות [בקרת הגישה המבוססות על תפקידים (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) לניהול משאבים במנוי יוסרו לצמיתות. רק לבעלים החדש תהיה גישה לניהול משאבים במנוי. לקבלת מידע נוסף, ראה [העברת מנוי למשתמש בדייר אחר של הודעה בנושא תכלת](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**העברת בעלות על מנוי**

גישה מודרישות מוקדמות של העברת מנויים בבעלות מנוי (RBAC) לניהול משאבים במנוי מאבדת את הגישה שלו. לקבלת מידע נוסף אודות הוספת מנוי קיים לדייר, ראה [שיוך או הוספת מנוי של תכלת לתכלת Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- העברת מנויים עם סכום מיוחד קיים ממחזור החיובים הנוכחי לא תועבר לכלי התשלום החדש בחשבון החדש. המידע היחיד הזמין למשתמשים בחשבון החדש הוא עלות החודש האחרון עבור המנוי שלך. שאר היסטוריית השימוש והחיוב אינה מעבירה עם המנוי.
- העברת בעלות על חיוב של מנויי הסכם Enterprise (EA) נתמכת כעת בפורטל הסכם הארגון בלבד
- העברת מנוי מונחה-אשראי כגון Visual Studio, BizSpark, הרשת השותפים של Microsoft למשתמש חדש מחייבת להיות בעל רשיון רשת של Visual Studio/Microsoft פרטנר כדי לקבל את בקשת ההעברה
- כל המשאבים כגון מחשבים וירטואליים, דיסקים ואתרי אינטרנט מועברות לחשבון החדש בהצלחה. המשאבים הבאים עשויים להיות מושפעים מהעברת מנויים בין דיירים:

**שירותים בתחום תכלת לספירה**

קמרונות מפתח תכלת

- [משתמשים קשורים ב-SQL ומסדי נתונים](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) עשויים להיות מושפעים, במיוחד אם הלקוח משתמש באימות הקשור בנושא תכלת של active Directory
- **שירותי יישומים שתצורתם** נקבעה באמצעות אימות Active Directory עשויים להיות מושפעים
- **צוות Visual Studio** חשבונות שירותים המחוברים למנויי תכלת עשויים לאבד את הגישה באופן זמני כאשר מנוי התכלת המחובר מבוטל

**מסמכים מומלצים**

שלבים לאחר קבלת בעלות על חיוב:

- כדי לשמור על בעלות על חיוב, אך לשנות את סוג המנוי שלך, עיין במאמר: [העבר את מנוי התכלת שלך להצעה אחרת](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [העברת Visual Studio, Microsoft Network Network (MPN) ושלם במהלך העבודה על Dev/בדיקת מנויים](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [העברת בעלות על חיוב עבור מנויי הסכם Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [שאלות נפוצות אודות העברת בעלות](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [פתרון בעיות בעלות העברה](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)