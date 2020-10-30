---
title: מדוע לחצן ' הוסף תקציב ' אינו זמין עבורי?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807409"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>מדוע לחצן ' הוסף תקציב ' אינו זמין עבורי?

כדי ליצור תקציב, דרושות לך אחת מההרשאות הבאות:

- קבוצת ניהול, מנויים, טווחי קבוצות משאבים
- משתתף ניהול עלויות
- בעלים
- שתתף '
- לקוח ארגוני בלבד: הרשמה, מחלקה, טווחי חשבון
- מנהל ההרשמה (הגדרת תקציב בטווח ההרשמה)
- מנהל מחלקה (הגדרת תקציב בטווח המחלקות)
- בעלים של חשבון (הגדרת תקציב בטווח חשבון)
- הסכם לקוח מודרני בלבד: חשבון חיוב, פרופיל חיוב, טווחי מקטע חשבונית
- יוצר מנויים של תכלת

**יצרתי תקציב כאשר עלותי עבור החודש הנוכחי כבר היתה חורגת מהתקציב. מדוע לא קיבלתי התראה?**  
אם כבר חרגת מ-סף עלות נתון בעת יצירת תקציב שהתראה זו לא תתבצע באש. לאחר שמחזור חדש מתחיל, אם אתה מפר את הסף, ההתראה יורה.

**מתי עליי לצפות לקבל התראה לאחר שחרגת מאחד מספי ההתראה המוגדרים בתקציב שלי?**  
תקציבים מוערכים כל 4 שעות. לוקח לפחות 8 שעות לשימוש בנתוני שימוש כדי להגיע למערכת התקציבים. בהינתן זאת, התראות עשויות להימשך כל עוד 12 שעות לאחר שתחרוג מהסף.

**מדוע לחצן ' תאריך התחלה ' אינו זמין כאשר אני בוחר את משך הזמן לאיפוס חודש או חיוב?**  
התקציבים מיושרים לחודש לוח השנה הנוכחי או לתקופת החיוב הנוכחית (במקרה שבו נבחר חודש החיוב). לכן, אנו מאכלסים מראש ערך זה עבורך.

**מדוע איני רואה גרף של העלויות שלי בחוויית יצירת התקציב?**  
אנו זקוקים למינימום של חודשיים של נתוני עלות לפני שנוכל לעבד גרף כדי לסייע לך ביצירת תקציב.

**מדוע אין באפשרותי להגדיר תקציב כנגד מנוי שיצרתי זה עתה?**  
לאחר יצירת מנוי, הנתונים לוקחים 24-48 שעות כדי לעבד לפני הגדרת תקציב נגדו.

**משאבי API של תקציב**

- [תקציבים של API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): מספק פעולות ליצירה ועדכון של תקציבים. באמצעות ה-API של תקציבים, באפשרותך להגדיר סף תקציב ולקבוע את התצורה של התראות מרובות לירי בעת הגישה לסף זה. התראות יכולות לגרום לדואר אלקטרוני או לקבוצת פעולות של תכלת לבצע אוטומציה. הערה: סינון עבור API זה אינו מתיישר עם סינון/ממדים של שאילתות API.
- [תקציבים של API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): יצירת תקציבים בעלי יכולות סינון עלות גבוהה יותר מאשר v1. סינון מיושר לחוזה המשמש בממשקי Api של שאילתות וממדים. זהו ה-API המומלץ של תקציבים לשימוש במעבר קדימה.
- [ממדים](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): מספק פעולות לקבלת ממדים נתמכים עבור השימוש שלך תחת מגוון רחב של טווחים. באמצעות API של ממדים, באפשרותך לאחזר רשימת ממדים שניתן להשתמש בהם כקלט ליצירת שאילתות באמצעות ה-API של השאילתה.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): מספק פעולות כדי לקבל עלויות צבורות ונתוני שימוש בהתבסס על השאילתה שאתה מספק. באמצעות ה-API של השאילתה, באפשרותך לציין את הסינון, המיון והקיבוץ הרצויים בכל הממדים הזמינים (שאליהם יש גישה מממשק API של ממדים).

**עלויות חזויות**

**מדוע איני רואה תחזיות עבור העלויות שלי בניתוח עלות?**  
יש כמה סיבות אפשריות לכך שתחזית התחזית חסרה עבורך בניתוח עלות, חלק מהן הן כדלקמן:

1. אם נתוני העלות שלך בני פחות מ-10 ימים, התרשים החזוי לא ייטען. המודל מחייב לפחות 10 ימים של נתוני עלות אחרונים לתחזיות מדויקות
2. אם בחרת תאריכים היסטוריים, התרשים החזוי לא יהיה גלוי. בחר טווח תאריכים עם תאריכים עתידיים להצגת התרשים החזוי
3. אם החשבון שלך כולל מטבעות מרובים, התרשים החזוי יכלול רק את העלויות של ' כל העלויות ב-USD '

**מדוע התחזית אינה משתנה כאשר אני מבצע שינויים במשאבים שלי?**  
מודל התחזית מחייב כמה ימים לחשבון שינויים בחשבון ואינו מבצע הקרנה מיידית בהתבסס על שינוי במשאבים  
לקבלת שלבים גדולים יותר של הגדלה או הקטנה של משאבים, המודל ייקח מעט זמן רב יותר להסתגל לשינויים אלה כדי להתחשב בסטיות

**מדוע התחזית שלי גדלה לאחר שאני מבצע רכישה של הזמנות או שוק?**  
מודל התחזית מחשיב את ' העלות בפועל ' ואינו מסביר שימוש ורכישה בנפרד. לרכישה חד-פעמית, המודל יקטין את התחזיות לאחר 10 ימים לחשבון העלייה הפתאומית בעלויות

**אני רוצה לראות תחזיות עבור מימד אחד (למשל. מד ה**  
התחזית תומכת כעת בתחזיות עלות כוללת ולא עבור מטרים בודדים. מכאן, כאשר ' מקובצות לפי ' ממד, התחזיות יהיו עבור סך כל הפריטים בממד

**מסמכים מומלצים**

- [מהו ניהול עלות של תכלת?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [שיטות עבודה מומלצות לניהול עלות של תכלת](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ניתוח עלויות והוצאות](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [סיור וניתוח עלויות באמצעות ' ניתוח עלות '](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ניהול עלות של תכלת: תמחור](https://azure.microsoft.com/services/cost-management/#pricing)
- [סקירת עלויות בניתוח עלות](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [ערכת לימוד של וידאו: יצירת תקציב בפורטל תכלת](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [דרישות מוקדמות לצורך הצגה והתאמה אישית של תקציבים](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [יצירה וניהול של תקציבים](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [קביעת תצורה של אוטומציה באמצעות האפשרות ' קבוצות פעולה של תכלת ותקציבים '](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [שימוש בהתראות עלות כדי לנטר שימוש והוצאות](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [שיטות עבודה מומלצות לניהול עלויות](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**סרטוני וידאו של ערכת לימוד**

- [יצירת תקציב בפורטל ' תכלת '](https://go.microsoft.com/fwlink/?linkid=2146761)
- [ניהול עלויות באמצעות API של תקציבים וקבוצות פעולה](https://go.microsoft.com/fwlink/?linkid=2147038)