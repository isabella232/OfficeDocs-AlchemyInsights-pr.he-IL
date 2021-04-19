---
title: סוגי מנויים נתמכים
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820683"
---
# <a name="supported-subscription-types"></a>סוגי מנויים נתמכים

עיין בסוגי המנויים הנתמכים כדי להמשיך הלאה.

[סוגי מנויים נתמכים](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**העברת בעלות על חיוב**

Azure portal כמנהל [החשבון](https://ms.portal.azure.com/) של חשבון החיוב הכולל את המנוי שברצונך להעביר

- חפש ב **ניהול עלויות + חיוב**. בחר **מנויים** מהחלונית הימנית. בהתאם לגישה, ייתכן שתצטרך לבחור טווח חיובים ולאחר מכן לבחור **מנויים** או **מנויי Azure**.
- בחר העבר בעלות על חיוב עבור המנוי שברצונך להעביר
- הזן את כתובת הדואר האלקטרוני של משתמש שהוא מנהל חיוב של החשבון אשר יהיה הבעלים החדש של המנוי ולאחר מכן בחר **שלח בקשת העברה**
- המשתמש מקבל הודעות דואר אלקטרוני כולל הוראות לסקירת בקשת ההעברה. כדי לאשר את בקשת ההעברה, המשתמש בוחר את הקישור בהודעת הדואר האלקטרוני ופועל לפי ההוראות.

הערה: אם אתה מעביר בעלות חיוב על המנוי שלך לחשבון של משתמש בדייר אחר של Azure AD, כל ההקצאות של בקרת גישה [מבוססת תפקידים (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) לניהול משאבים במנוי מוסרות לצמיתות. רק לבעלים החדש תהיה גישה לניהול משאבים במנוי. לקבלת מידע נוסף, [ראה העברת מנוי למשתמש דייר Azure AD אחר](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**העברת בעלות על מנוי**

העברת תנאים מוקדמים להעברת בעלות על מנוי על גישה מבוססת תפקיד (RBAC) כדי לנהל משאבים במנוי מאבדים את הגישה שלהם. לקבלת מידע נוסף אודות הוספת מנוי קיים לדייר, ראה שיוך [או הוספה של מנוי Azure ל- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- העברת מנוי עם סכום יוצא דופן קיים ממחזור החיוב הנוכחי לא יועבר לכלי התשלום החדש בחשבון החדש. המידע היחיד הזמין למשתמשים בחשבון חדש הוא העלות של החודש האחרון עבור המנוי שלך. שאר היסטוריית השימוש וחיוב אינה מעבירה עם המנוי.
- העברת בעלות חיוב על מנויי הסכם ארגוני (EA) נתמכת בשלב זה בפורטל הסכם ארגוני בלבד
- העברת מנוי מונחה אשראי, כמו Visual Studio, BizSpark, רשת השותפים של Microsoft למשתמש חדש דורשת רשיון רשת של שותף Visual Studio/Microsoft כדי לקבל את בקשת ההעברה
- כל המשאבים, כמו מחשבים וירטואליים, דיסקים ואתרי אינטרנט, יועברו לחשבון החדש בהצלחה. ייתכן שהמשאבים הבאים יושפעו בהעברת מנוי בין דיירים:

**Azure AD Domain Services**

Azure Key Vaults

- [המשתמשים ומסדי הנתונים הקשורים](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) ל- SQL יכולים להיות מושפעים, במיוחד אם הלקוח משתמש באימות קשור של Azure Active Directory
- **ייתכן ש'שירותי** יישום' שתצורתם נקבעה באמצעות אימות Azure Active Directory
- **צוות Visual Studio** חשבונות שירותים המחוברים למנויים של Azure עשויים לאבד באופן זמני את הגישה כאשר המנוי המחובר של Azure מבוטל

**מסמכים מומלצים**

שלבים לאחר קבלת בעלות על חיוב:

- כדי לשמור על בעלות על חיוב, אך לשנות את סוג המנוי שלך, עיין: [החלפת המנוי שלך ב- Azure להצעה אחרת](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [מנויי פיתוח/בדיקה של העברת Visual Studio,‏רשת השותפים של Microsoft (MPN) ושלם תוך כדי תנועה](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [העברת בעלות חיוב על מנויי הסכם ארגוני (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [שאלות נפוצות אודות העברת בעלות](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [פתרון בעיות של העברת בעלות](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)