---
title: מדוע לחצן הוסף תקציב אינו זמין עבורי?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822636"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>מדוע לחצן הוסף תקציב אינו זמין עבורי?

כדי ליצור תקציב, עליך לקבל אחת מההרשאות הבאות:

- ניהול קבוצה, מנוי, טווחי קבוצת משאבים
- משתתף בניהול עלויות
- בעלים
- משתתף
- לקוח ארגוני בלבד: הרשמה, מחלקה, טווחי חשבון
- מנהל הרשמה (הגדרת תקציב בטווח ההרשמה)
- מנהל מחלקה (הגדרת תקציב בטווח המחלקה)
- בעלים של חשבון (הגדרת תקציב בטווח חשבון)
- הסכם לקוח מודרני בלבד: חשבון חיוב, פרופיל חיוב, טווחי מקטע חשבונית
- יוצר המנוי של Azure

**יצרתי תקציב כאשר העלות שלי עבור החודש הנוכחי כבר היתה מעבר לתקציב. מדוע לא קיבלתי התראה?**  
אם כבר חרגת מסף עלות נתון בעת יצירת תקציב שהתראה זו לא תידלק. לאחר תחילת מחזור חדש, אם תפרוץ את הסף, ההתראה תיתחיל.

**מתי עליי לצפות לקבל התראה לאחר שאחרם על אחד מסספי התראת התקציב המוגדרים שלי?**  
התקציבים מוערכים כל 4 שעות. נדרשות לפחות 8 שעות עד שנתונים של שימוש יגיעו למערכת התקציבים. בהתחשב בתאריך זה, ייתכן ש- 12 שעות עד ש- 12 שעות יעלו על סף.

**מדוע לחצן 'תאריך התחלה' אינו זמין כאשר אני בוחר תקופת איפוס לחודש או לחיוב?**  
התקציבים מיושרים לחודש לוח השנה הנוכחי או לתקופת החיוב הנוכחית (במקרה שבו נבחר 'חודש חיוב'). לכן, אנו מאכלסים מראש ערך זה בשבילך.

**מדוע איני רואה גרף של העלויות שלי בחוויה ליצירת תקציב?**  
אנו זקוקים למינימום של חודשיים של נתוני עלות כדי שנוכל לעבד גרף כדי לסייע לך ביצירת תקציב.

**מדוע איני יכול להגדיר תקציב מול מנוי שיצרתי זה עתה?**  
לאחר יצירת מנוי, נדרשות 24-48 שעות לעבד את הנתונים לפני הגדרת תקציב כנגדו.

**משאבי API של תקציב**

- [Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): מספק פעולות ליצירה ולעדכון של תקציבים. באמצעות ה- API של תקציבים, באפשרותך להגדיר סף תקציב ולקבוע תצורה של התראות מרובות כך שתשתמש בגישה לסף זה. התראות יכולות להפעיל הודעת דואר אלקטרוני או קבוצת פעולות של Azure כדי לבצע אוטומציה. הערה: סינון עבור API זה אינו תואם לסינון/ממדים של API של שאילתה.
- [Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): צור תקציבים עם יכולות סינון עלויות גבוהות יותר מ- v1. סינון יישור לחוזה המשמש ב- API של השאילתות והממדים שלנו. זהו ה- API של התקציבים המומלצים לשימוש בתנועה קדימה.
- [ממדים](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): מספק פעולות לקבלת ממדים נתמכים עבור השימוש שלך תחת מגוון טווחים. באמצעות ה- API של הממדים, באפשרותך לאחזר רשימה של ממדים ה יכולים לשמש כקלט ליצירת שאילתות באמצעות ה- API של השאילתה.
- [שאילתה](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): מספק פעולות כדי לקבל נתוני עלות ושימוש מצטברים בהתבסס על השאילתה שאתה מספק. באמצעות ה- API של השאילתה, באפשרותך לציין את הסינון, המיון והקיבוץ הרצויים בכל הממדים הזמינים (שה- API של הממדים ניגשים אליו).

**עלויות תחזית**

**מדוע איני רואה תחזיות עבור העלויות שלי בניתוח עלות?**  
ישנן סיבות מרובות לכך שההתחזית עשויה להיות חסרה בהן בניתוח עלות, חלקן הן כדלקמן:

1. אם נתוני העלות שלך ישנים פחות מ- 10 ימים, תרשים התחזית לא ייטען. המודל דורש לפחות 10 ימים של נתוני עלות אחרונים עבור תחזיות מדויקות
2. אם בחרת תאריכים היסטוריים, תרשים התחזית לא יהיה גלוי. בחר טווח תאריכים עם תאריכים עתידיים להצגה של תרשים התחזית
3. אם החשבון שלך כולל מטבעות מרובים, תרשים התחזית יפרוייקט רק עלויות עבור 'כל העלויות ב- USD'

**מדוע התחזית אינה משתנה בעת ביצוע שינויים במשאבים שלי?**  
מודל התחזית דורש כמה ימים כדי לתת חשבון לשינויים בחשבון ולא לבצע תחזיות מיידיות בהתבסס על שינוי במשאבים  
לקבלת שלבים גדולים יותר של הגדלה או הקטנה במשאבים, ההסתגלות של המודל לשינויים אלה תתבצע בחשבון חריגות

**מדוע התחזית שלי גדלה לאחר ביצוע הזמנה או רכישת Marketplace?**  
מודל התחזית מתייחס ל'עלות בפועל' שלך ולא מתייחס לשימוש ולרכישה בנפרד. עבור רכישה של פעם אחת, המודל יפחית את התחזיות לאחר 10 ימים כדי לתת חשבון לגידול הפתאומי בעלויות

**אני רוצה לראות תחזיות עבור ממד יחיד (לדוגמה. Meter)**  
התחזית תומכת כעת בהתחזיות עלות כוללות ולא במטרים בודדים. מכאן, כאשר 'מקובצים לפי' ממד, התחזיות יהיו עבור סך כל הפריטים בממד

**מסמכים מומלצים**

- [מהו Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [שיטות עבודה מומלצות לניהול עלויות של Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ניתוח העלויות וההוצאות שלך](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [חקור ונתח עלויות באמצעות ניתוח עלות](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ניהול עלויות של Azure: תמחור](https://azure.microsoft.com/services/cost-management/#pricing)
- [סקירת עלויות בניתוח עלות](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [ערכת לימוד בנושא וידאו: יצירת תקציב בפורטל Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [דרישות מוקדמות להצגה ולהתאמה אישית של תקציבים](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [יצירה וניהול של תקציבים](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [קביעת תצורה של אוטומציה עם Azure Action Groups ו- API של תקציבים](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [שימוש בהתראות עלות כדי לנטר שימוש והוצאות](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [שיטות עבודה מומלצות לניהול עלויות](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**סרטוני הדרכה**

- [יצירת תקציב בפורטל Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [ניהול עלויות באמצעות ה- API של תקציבים וקבוצות פעולה](https://go.microsoft.com/fwlink/?linkid=2147038)