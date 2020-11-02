---
title: רכישת מופע של חיוב עבור מופע שמור
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823076"
---
# <a name="billing-for-reserved-instance-purchase"></a>רכישת מופע של חיוב עבור מופע שמור

רכישת המופע השמור מחויבת לשיטת התשלום הקשורה למנוי שבחרת בזמן הרכישה. סוג המנוי חייב להיות הסכם ארגוני (מספר הצעה: MS-AZR-0017P), תשלום לפי-לך-Go (הצעה מספר: MS-AZR-0003P), הסכם לקוח של Microsoft או CSP.

- עבור מנוי ארגוני, החיובים מנוכה מיתרת המחויבות המוניטרית של ההרשמה או מחויבת להיטען
- עבור מנוי בתשלום כפי שתרצה, החיובים מחויבים לשיטת התשלום של כרטיס האשראי או החשבונית במנוי

**ביטול הזמנה**

- **שירות עצמי:** באפשרותך לבטל או להחליף מופע שמור בעצמך באמצעות [הפורטל התכלת](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנה ולחץ על החזר או על exchange. שים לב שעליך להיות בעל גישה לבעלים בהזמנת ההזמנה כדי לבצע החלפה או החזר. גישה רק להזמנה לא תאפשר לך להמשיך בהחזר או ב-exchange. בקש מהבעלים של הזמנת ההזמנות להעניק לך גישה לבעלים להזמנת ההזמנה
- **מדיניות Exchange:** באפשרותך להחליף הזמנה להזמנה אחרת מאותו סוג – אין **קנסות** על חילופי הזמנות. המחויבות הכוללת של ההזמנה החדשה צריכה להיות גדולה יותר מהסכום של סכום ההחזר של ההזמנה שחלפה והתשלומים החודשיים העתידיים (אם ישים)
- **מדיניות החזר:** סכום ההחזר הכספי והתשלומים העתידיים שבוטלו אינם יכולים לחרוג מ-$50,000 USD בחלון מתגלגל של 12 חודשים. אנחנו **לא גובים כל עונש** על החזרים, אך הם יכולים לחייב אותו על החזרים עתידיים

**חריגים:** יכולת exchange וביטול של שירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני של ממשלת ארה"ב

- התמיכה ב- **API/PS/CLI** אינה זמינה לביטול ולזיכוי [של חילופים והחזרים בשירות עצמי עבור הזמנות של שירותים בתכלת](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- יכולת exchange וביטול של שירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני של ממשלת ארה"ב. סוגי מנויים אחרים של ממשלת ארצות הברית, כולל התמיכה בתשלום-לפי-לך ובCSP

[מידע נוסף: אופן העיבוד של טרנזקציות return ו-exchange מידע](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) נוסף: [exchange והחזר מדיניות](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) שאלות נוספות: [בקר במסמכי מופע שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**החלפת מופע שמור קיים (שירות עצמי)**

באפשרותך להחליף הזמנה להזמנה אחרת מאותו סוג. באפשרותך גם להחזיר הזמנה, עד $50,000 USD בשנה, אם אינך זקוק לה עוד. יכולת exchange וביטול של שירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני של ממשלת ארה"ב. סוגי מנויים אחרים של ארצות הברית, כולל התמיכה בתשלום לפי-הנסיעה ו-CSP. עליך להיות בעל גישה לבעלים בהזמנת ההזמנה כדי להחליף או להחזיר הזמנה קיימת.

השלבים הבאים ינחו לגבי ההליך להשלמת הטרנזקציה

1. היכנס [לפורטל התכלת](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנות שברצונך להחזיר ולחץ על **Exchange** 2. בחר את מוצר ה-VM שברצונך לרכוש והקלד כמות. ודא שסכום הרכישה החדש הוא יותר מסכום ההחזרה [הקובע את הגודל הנכון לפני הרכישה](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. סקור והשלם את הטרנזקציה

**החזר כספי עבור מופע שמור**

כדי להחזיר הזמנה, עבור אל **פרטי ההזמנה** ולחץ על **החזר כספי**

**החזר Pro-מדורג:**

**דוגמאות לדרישת מינימום ודרישות מינימום להחזר ולהחלפה** דוגמה להזמנה מראש:

- באפשרותך לרכוש RI של שנה אחת עבור $120 ב-1 בינואר
- ב-7 באפריל ברצונך לקבל החזר או להחליף הזמנה זו
- מאחר שההזמנה חיה במשך 97 ימים, תקבל (1-97/365) * $120 בחזרה. (i.e. $88.1). אין כרגע עונש על החזרים
- אם החלפת הרכוש, הרכישה החדשה צריכה להיות גדולה מ-$88.1
- אין כל עונש על החזרים כרגע

**דוגמה להזמנה לתוכנית חיוב:**

- באפשרותך לרכוש רי מונח של שנה אחת עבור $10 לכל חודש
- ב-7 באפריל ברצונך לקבל החזר או להחליף הזמנה זו
- מאחר שהתשלום האחרון אירע 7 ימים, תקבל (1-7/31) * $10 בחזרה. (לדוגמה, $7.74)
- התשלומים העתידיים שבוטלו הם $80. אין כרגע עונש על החזרים
- ביטול זה יפחית את הנכות של $87.74 שאתה מגבלת $50,000 ההחזר
- אם החלפת, הערך הכולל של רכישה חדשה אמור להיות גדול מ-$87.74

**לא ניתן לראות חשבונית עבור תקופת החיוב האחרונה**

כמה סיבות אפשריות לכך שייתכן שלא תראה חשבונית:

- יש לך כמות אשראי חודשית עם המנוי שלך שלא חרגת ממנו או אם יש לך גירסת ניסיון ללא תשלום. חשבונית נוצרת רק כאשר אתה חייב כסף
- זה פחות מ-30 יום מהיום שבו נרשמת כמנוי לתכלת
- החשבונית אינה מופקת עדיין. המתן עד לסיום תקופת החיוב
- אם אינך מנהל החשבון, ייתכן שהחשבוניות הקודמות לא יהיו זמינות עבורך

**הורדת החשבונית שלך מפורטל התכלת (. pdf)**

- בחר את המנוי שלך מהדף ' [מנויים](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ' בפורטל התכלת [כמשתמש עם גישה לחשבוניות](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- בחירת **חשבוניות**
- לחץ על **הורד חשבונית** כדי להציג עותק של חשבונית ה-PDF שלך. אם ההודעה **אינה זמינה** , ראה [מדוע איני רואה חשבונית עבור תקופת החיוב האחרונה?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**קבלת החשבונית שלך בדואר אלקטרוני (. pdf)**

- בחר את המנוי שלך מהדף ' [מנויים](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) '. לחץ על **חשבוניות** ולאחר מכן שלח בדואר אלקטרוני את החשבונית שלי
- לחץ על **הצטרפות** וקבל את התנאים. יהיה עליך להצטרף עבור כל מנוי שבבעלותך

הערה: אם אינך מקבל הודעת דואר אלקטרוני לאחר ביצוע השלבים, ודא שכתובת הדואר האלקטרוני שלך נכונה [בהעדפות התקשורת בפרופיל שלך](https://account.windowsazure.com/profile)

**הורדת נתוני השימוש שלך מפורטל התכלת**

- כניסה [למרכז החשבון](https://account.windowsazure.com/Subscriptions) של תכלת [כמנהל החשבון](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- בחר את המנוי שעבורו ברצונך לקבל את פרטי החשבונית והשימוש
- בחר **היסטוריית חיוב**
- בחר באפשרות **הצג משפט נוכחי** כדי לראות הערכה של החיובים שלך בזמן שההערכה נוצרה
- בחר **הורד שימוש** כדי להוריד את נתוני השימוש היומיים כקובץ CSV. אם אתה רואה שתי גירסאות זמינות, הורד את גירסה 2

שאלות נוספות: [בקר במסמכי מופע שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**מסמכים מומלצים**

- [יסודות החיוב](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הכרת אופן ההחלה של הנחת המופע השמור](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הורדה או הצגה של חשבונית החיוב של התכלת ונתוני השימוש היומיומיים](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הכרת אופן ההחלה של הנחת המופע השמור](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הכרת השימוש במופעים השמורים עבור מנוי התשלום כפי שאתה עושה](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הכרת השימוש במופע השמור עבור הרשמת הארגון שלך](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [עלויות תוכנה של Windows שאינן כלולות במופעים שמורים](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [המופעים השמורים בתוכנית ספק פתרונות הענן המרכזי של השותפים (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)