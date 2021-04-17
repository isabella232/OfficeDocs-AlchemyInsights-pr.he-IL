---
title: חיוב עבור רכישה של מופע שמור
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
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820323"
---
# <a name="billing-for-reserved-instance-purchase"></a>חיוב עבור רכישה של מופע שמור

הרכישה של המופע השמור מחויבת בשיטת התשלום הקשורה למנוי שתבחר בעת הרכישה. סוג המנוי חייב להיות הסכם ארגוני (מספר הצעה: MS-AZR-0017P), Pay-As-You-Go (מספר הצעה: MS-AZR-0003P), הסכם הלקוח של Microsoft או CSP.

- עבור מנוי ארגוני, החיובים מנוקטים מהיתרה של ההתחייבות המוניוטרית של ההרשמה או מחויבים כתשלום יתר
- עבור מנוי Pay-As-You-Go, החיובים חויבו בכרטיס האשראי או בשיטת התשלום בחשבונית במנוי

**ביטול ההזמנה**

- **שירות עצמי:** באפשרותך לבטל או להחליף מופע שמור בעצמך באמצעות [פורטל Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנה ולחץ על החזר או על החלפה. שים לב כי עליך לקבל גישה לבעלים בהזמנה כדי להחליף או להחזיר. Access רק ההזמנה לא תיתן לך להמשיך עם החזר או החלפה. בקש מהבעלים של הזמנת ההזמנה להעניק לך גישה לבעלים להזמנה
- **מדיניות Exchange:** ניתן להחליף הזמנה עבור הזמנה אחרת מאותו סוג – אין קנסות **בחילופי** הזמנות. ההתחייבות הכוללת עם הזמנה חדשה צריכה להיות גדולה מסכום ההחזר של ההזמנה ההחלפה והתשלום החודשי העתידי (אם ישים)
- **מדיניות החזר:** סכום ההחזר והתשלום העתידי שבוטלו אינם יכולים לעלות על 50,000 דולר בחלון גלגול של 12 חודשים. בשלב **זה, איננו מחייבים קנס על** החזרים, אך אנו יכולים לחייב אותו על החזרים עתידיים

**חריגות:** יכולת החלפה וביטול בשירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני ממשלתי של ארה"ב

- **תמיכה ב- API / PS / CLI** אינה זמינה עבור ביטולים והחזרים של החליפין בשירות עצמי [והחזרים כספיים עבור Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- יכולת החלפה וביטול בשירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני ממשלתי של ארה"ב. סוגי מנויים אחרים של ממשלת ארה"ב, כולל Pay-As-You-Go ו- CSP, נתמכים

קבל מידע נוסף : [כיצד מתבצע עיבוד של עסקאות](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) החזרה וחילופי מידע נוסף : מדיניות [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) והחזר שאלות נוספות: בקר במסמך [מופעים שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**החלפת מופע שמור קיים (שירות עצמי)**

באפשרותך להחליף הזמנה עבור הזמנה אחרת מאותו סוג. באפשרותך גם להחזיר הזמנה, עד 50,000 דולר לשנה, אם אינך זקוק לה עוד. יכולת החלפה וביטול בשירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני ממשלתי של ארה"ב. סוגי מנויים אחרים של ממשלת ארה"ב, כולל Pay-As-You-Go ו- CSP, נתמכים. כדי להחליף או להחזיר הזמנה קיימת, עליך לקבל גישה לבעלים בהזמנה.

השלבים הבאים מדריכים את ההליך להשלמת העסקה

1.היכנס לפורטל [Azure שלך.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) בחר את ההזמנות שברצונך להחזיר ולחץ על **Exchange** 2.בחר את מוצר ה- VM שברצונך לרכוש והקלד כמות. ודא שסכום הרכישה החדש גדול מסכום ההחזרה [קבע את הגודל הנכון לפני הרכישה.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.סקור והשלם את העסקה

**החזר עבור מופע שמור**

כדי להחזיר הזמנה, עבור אל פרטי **ההזמנה ולחץ** על **החזר**

**החזר פרו-דירוג:**

**דוגמאות לדרישות Pro-ration ודרישות מינימליות עבור החזר והחלפה** דוגמה להזמנה מראש:

- אתה רוכש RI לשנה אחת עבור $120 ב- 1 בינואר
- ב- 7 באפריל ברצונך להחזיר או להחליף הזמנה זו
- מאחר שה ההזמנה חיה במשך 97 ימים, אתה מקבל (1-97/365) * $120 בחזרה. (כלומר$ 88.1). בשלב זה אין קנס על החזרים
- אם אתה מחליף, הרכישה החדשה צריכה להיות גדולה מ- $88.1
- אין קנס על החזרים בשלב זה

**דוגמה להזמנה של תוכנית חיוב:**

- אתה רוכש RI לשנה אחת עבור $10 לחודש
- ב- 7 באפריל ברצונך להחזיר או להחליף הזמנה זו
- מאחר שהתשלום האחרון התרחש 7 ימים, אתה מקבל (1-7/31) * $10 בחזרה. (כלומר$ 7.74)
- התשלומים העתידיים שבוטלו הם 80 $. בשלב זה אין קנס על החזרים
- ביטול זה יכוך $87.74 ממגבלת ההחזר בסך $50,000
- אם אתה מחליף, הערך הכולל של רכישה חדשה אמור להיות גדול מ- $87.74

**לא ניתן לראות חשבונית עבור תקופת החיוב האחרונה**

כמה סיבות אפשריות לכך שלא תראה חשבונית:

- יש לך סכום אשראי חודשי עם המנוי שלך שלא לחרוג או שיש לך גירסת ניסיון ללא תשלום. חשבונית נוצרת רק כאשר אתה חייב כסף
- עברו פחות מ- 30 יום מהיום שבו נרשמת כמנוי ל- Azure
- החשבונית עדיין לא נוצרה. המתן עד סוף תקופת החיוב
- אם אינך מנהל החשבון, ייתכן שחשבוניות ישנות יותר לא יהיו זמינות לך

**הורד את החשבונית שלך מפורטל Azure ( .pdf)**

- בחר את המנוי שלך [מהדף מנויים](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) בפורטל Azure [כמשתמש בעל גישה לחשבוניות](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- בחר **חשבוניות**
- לחץ **על הורד חשבונית** כדי להציג עותק של חשבונית ה- PDF שלך. אם כתוב **"לא זמין",** ראה מדוע איני רואה [חשבונית עבור תקופת החיוב האחרונה?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**קבלת החשבונית בדואר אלקטרוני ( .pdf)**

- בחר את המנוי שלך [מהדף מנויים.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) לחץ **על חשבוניות ולאחר מכן** שלח את החשבונית שלי בדואר אלקטרוני
- לחץ **על ההצטרפות** וקבל את התנאים. יהיה עליך להצטרף לכל מנוי בבעלותך

הערה: אם אינך מקבל הודעת דואר אלקטרוני לאחר ביצוע השלבים, ודא שכתובת הדואר האלקטרוני שלך נכונה [בהעדפות התקשורת בפרופיל שלך](https://account.windowsazure.com/profile)

**הורד את נתוני השימוש שלך בפורטל Azure**

- היכנס למרכז [החשבון של Azure כמנהל](https://account.windowsazure.com/Subscriptions) [החשבון](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- בחר את המנוי שעבורו ברצונך לקבל את פרטי החשבונית והשימוש
- בחר **היסטוריית חיובים**
- בחר **הצג משפט נוכחי** כדי לראות הערכה של החיובים שלך בעת יצירת ההערכה
- בחר **הורד שימוש** כדי להוריד את נתוני השימוש היומיים כקובץ CSV. אם אתה רואה שתי גירסאות זמינות, הורד את גירסה 2

שאלות אחרות: [בקר במסמך מופעים שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**מסמכים מומלצים**

- [יסודות החיוב](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת אופן ההחלה של הנחת מופע שמור](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הורדה או הצגה של חשבונית החיוב של Azure וניתוני שימוש יומיים](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת אופן ההחלה של הנחת מופע שמור](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת השימוש במופע שמור עבור מנוי Pay-As-You-Go שלך](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת השימוש במופע שמור עבור ההרשמה שלך לארגון](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [עלויות התוכנה של Windows אינן כלולות במופעים שמורים](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [מופעים שמורים בתוכנית ספק פתרונות ענן מרכזי שותף (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)