---
title: אני נחסם על-ידי גישה מותנית עם התקן המצורף לתחום
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036698"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>אני נחסם על-ידי גישה מותנית עם התקן המצורף לתחום

**כלים מומלצים במיוחד**

[כלי פותר בעיות של רישום מכשירים](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -הכלי שעוזר לפתור בעיות בבעיות רישום המכשירים הנפוצות ביותר.

[בדיקת קובץ script של קישוריות לרישום מכשירים](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -קובץ ה-script שעוזר להבטיח שההתקן יוכל לגשת לנקודות קצה של רישום מכשירים תחת חשבון המערכת.

[קובץ script לניקוי התקן תכלת](https://github.com/mzmaili/AzureADDeviceCleanup) -קובץ ה-script המאפשר לך לחפש ולנהל מכשירים ישנים בסביבה שלך.

להלן כמה סיבות נפוצות לכך שגישה מותנית עשויה להיכשל במכשיר שהצטרף לתחום (תכלת לספירה).

1. אין **כPRT מודעות מיידיות במכשיר** -עליך להבטיח שההתקן כולל אסימון רענון ראשי של הודעות מיידיות (PRT). לקבלת מידע נוסף אודות PRT, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)זה.

כדי לוודא אם יש לך תכלת AD PRT, באפשרותך לבצע `dsregcmd/status` את הפקודה במכשיר ולוודא אם "AzureAdPrt" שווה ל-"כן".

אם "AzureAdPrt" הוא "NO", בדוק את הפרטים הבאים:

- **בין אם יש לך סביבה מאוחדת עם AD FS, והיא אינה ניתנת לגישה מרשתות הבית של המשתמשים שלך**: במקרה זה, ודא שנקודות הקצה של usernamemixed "נגישות מהאקסטרא. אם הפרסום שלך ב-AD FS ממוקם מאחורי VPN, ודא שהמשתמשים מתחברים אל ה-VPN וכניסה מחדש למכשיר. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)זה.

- **אם ה-TPM של ההתקן פגום, ולכן אין לו אפשרות לאמת את ההתקן**: סמן את התיבה "tpm. msc" כדי לבדוק אם המצב של tpm הוא "מוכן". אם לא, `dsregcmd/leave` הפעל ותן להתקן להצטרף מחדש ל-תכלת AD. לאחר מכן, נסה שוב. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)זה.

- **אתה משתמש בספק זהויות של צד שלישי, שאינו תומך בפרוטוקול WS-Trust**. כפי שמתואר במסמכים שלנו, המכשירים ההיברידיים של תכלת לספירה אינם יכולים לפעול במקרה זה. בבקשה עבוד עם ספק הזהויות שלך לתמיכה.

2. **המשתמשים משתמשים בדפדפן Chrome ללא חשבונות Windows 10** או **שהסיומת של Office chrome אינם משתמשים באופן אוטומטי ב-PRT במכשירים המצורפים ל-או במכשירים** הקשורים ל-: פעולה זו מובילה לכישלון של כל מדיניות גישה מותנית מבוססת מכשיר, כאשר הודעת השגיאה ' התקן לא רשום ' מוצג. כדי להשתמש בדפדפן Chrome כראוי, עליך להתקין את ' חשבונות Windows 10 ' או ' הרחבת Office לדפדפן Chrome של המשתמשים ' דרך SCCM או כוונון. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)זה.

אם לא ניתן לדחוף את הסיומת מרחוק, הודע למשתמשים להתקין באופן ידני אחת מההרחבות שלעיל כדי לגשת ליישומים מאחורי גישה מותנית מבוססת מכשיר. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)זה.

3. **המכשיר היה כהלכה היברידית תכלת כלפי מעלה, אך היא נמחקה בטעות או הפכה ללא זמינה, עקב שינויים בסינכרון ב-תכלת AD Connect או מפורטל תכלת**: אם זה קורה, אובייקט ההתקן אינו מזוהה עוד כמכשיר המצורף לחלוטין, למרות שמצב "AzureAdJoined" ו-"PRT" מופיעים כחוקיים במכשיר.

כדי לפתור בעיה זו, `dsregcmd/leave` הפעל את המכשירים המושפעים והרשה להם להצטרף מחדש לתכלת לספירה. לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)זה.

> [!NOTE]
> אם המכשירים שלך נמצאים ב-Windows 10, 1809 update, באמצעות VPN/ענן Proxy וראה בעיות במצב "AzureAdPrt" או ביישום כלשהו עם בעיית SSO (outlook אינו מתחבר לתיבת דואר למרות שברשותך PRT), ודא שברשותך תיקון [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) או מצטבר של [עדכון מצטבר](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) כדי למנוע כשלים של PRT במכשירים אלה

















