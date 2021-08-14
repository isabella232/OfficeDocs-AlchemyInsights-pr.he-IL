---
title: Privileged Identity Management זה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973230"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management (PIM) תפקיד

**הרשאות לא מוענקות לאחר הפעלת תפקיד**

בעת הפעלת תפקיד ב- Azure AD Privileged Identity Management (PIM), ייתכן שההפעלה לא תפצה באופן מיידי לכל הפורטלים הדורשים את התפקיד ההרשאות. לעתים, גם אם השינוי מופצ, אחסון באינטרנט בפורטל עלול לגרום לשינוי שלא יתוקף באופן מיידי.

אם ההפעלה מתעכבת, בצע את הפעולות הבאות:

1. צא מהפורטל Azure ולאחר מכן היכנס שוב. בעת הפעלת תפקיד Azure AD או תפקיד משאב Azure, תראה את השלבים של ההפעלה. לאחר השלמת כל השלבים, תראה קישור 'צא'. באפשרותך להשתמש בקישור זה כדי לצאת. פעולה זו תפתור את רוב המקרים עבור השהיה בהפעלה.
2. ב- PIM, ודא שאתה מופיע כחבר בתפקיד.
3. אם אתה מפעיל את תפקיד מנהל Exchange, הקפד לצאת ולהירשם שוב. אם הבעיה נמשכת, פתח כרטיס תמיכה והגדל אותו כבעיה. אם אתה משתמש בתפקיד מנהל Exchange כדי לגשת למרכז האבטחה והתאימות, עיין בשלב הבא.
4. אם אתה מפעיל תפקיד לגישה למרכז האבטחה והתאימות או אם אתה מפעיל את תפקיד מנהל המערכת של SharePoint, תיתקל בעיכוב הפעלה מכמה דקות עד כמה שעות. זוהי בעיה ידועה ואנחנו עובדים עם צוותים אלה באופן פעיל כדי לפתור בעיה זו בהקדם האפשרי.

לקבלת מידע נוסף, ראה:

- [הפעלת תפקידי Azure AD שלי ב- PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [הפעלת תפקידי המשאב שלי ב- AZURE ב- PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**הרשאות לא יוסרו לאחר ביטול תפקיד או שתוקף הפעלת התפקיד יפוג**

בעת ביטול הפעלה של תפקיד ב- Azure AD Privileged Identity Management או כאשר תוקף תקופת הפעלת תפקיד פג, ייתכן שיש עיכוב שבו תמשיך לקבל גישה.

אם ביטול ההפעלות שלך מתעכב, בצע את הפעולות הבאות:

1. אם אתה מנפיק את תפקיד מנהל המערכת של Exchange או שתוקף תקופת הפעלת התפקיד פג, ואתה מבחין בעיכוב משמעותי לפני הסרת ההרשאות, פתח כרטיס תמיכה וספר למהנדס התמיכה שלך לעזור לך להגיש כרטיס עם צוות ניהול Access Privileged (PAM) בתוך Office אודות בעיה זו.
2. אם תוקף תקופת ההפעלה פג, אך הפעלת הדפדפן עדיין פתוחה, סגור את הדפדפן. באפשרותך להמשיך להשתמש בתפקיד עד שתסגור הפעלה זו. זוהי בעיה ידועה ואנחנו צופים בתיקון פוטנציאלי לבטל באופן פעיל כל הפעלה לאחר שתוקף ההפעלה פג.

אם ההשהיה שלך שונה משני תרחישים אלה, פתח כרטיס תמיכה.
