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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104021"
---
# <a name="billing-for-reserved-instance-purchase"></a>חיוב עבור רכישה של מופע שמור

הרכישה של מופע השמור מחויבת בשיטת התשלום הקשורה למנוי שאתה בוחר בזמן הרכישה. סוג המנוי חייב להיות הסכם ארגוני (מספר הצעה: MS-AZR-0017P), תשלום לפי שימוש (מספר ההצעה: MS-AZR-0003P), הסכם הלקוחות של Microsoft או ספק שירותי ה- CSP.

- עבור מנוי ארגוני, החיובים מופחתים מיתרת ההתחייבות הכספית של הרישום או מחויבים כתשלום עודף
- עבור מנוי תשלום לפי שימוש, החיובים מחויבים בכרטיס האשראי או שיטת תשלום החשבונית במנוי.

**ביטול הזמנה**

- **שירות עצמי: באפשרותך** לבטל או להחליף מופע שמור בעצמך באמצעות [פורטל Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנה ולחץ על החזר כספי או על Exchange. שים לב: כדי לבצע החלפה או החזר כספי, נדרשת גישת בעלים בהזמנה. גישה להזמנה בלבד לא תאפשר לך להמשיך בהחזר כספי או בהחלפה. בקש מהבעלים של ההזמנה להעניק לך גישת בעלים להזמנה
- **מדיניות החלפה:** באפשרותך להחליף הזמנה עבור הזמנה אחרת מאותו סוג – **אין קנסות** על החלפת הזמנה. ההתחייבות הכוללת להזמנה חדשה צריכה להיות גדולה יותר מסכום ההחזר עבור החלפת הזמנה וסכום התשלומים החודשיים העתידיים (אם רלוונטי)
- **מדיניות החזרים:** סכום ההחזר והתשלומים העתידיים שבוטלו אינם יכולים לעלות על 50,000 דולר בחלון פריסה של 12 חודשים. אנו לא **גובים כרגע קנסות** שניתנו על החזרים, אך ייתכן שנגבה אותם על החזרים עתידיים

**חריגים:** יכולת של החלפה בשירות עצמי וביטול אינה זמינה ללקוחות של ההסכם הארגוני הממשלתי של ארה"ב

- **תמיכת API / PS / CLI** אינה זמינה לביטול והחזרים [החלפות בשירות עצמי והחזרים עבור הזמנות Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- יכולת של החלפה בשירות עצמי וביטול אינה זמינה ללקוחות של ההסכם הארגוני הממשלתי של ארה"ב. סוגי מנויים אחרים של ממשלת ארה"ב, כולל Pay-As-You-Go ו- CSP נתמכים

קבל מידע נוסף : [כיצד מעובדות](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) עסקאות החזרה וחילופי מידע נוסף : [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) מדיניות החזר שאלות נוספות: בקר במסמך [מופעים שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**החלפת מופע שמור קיים (בשירות עצמי)**

באפשרותך להחליף הזמנה עבור הזמנה אחרת מאותו סוג. תוכל גם להחזיר תשלום על הזמנה, בסכום של 50,000 דולר לכל היותר בשנה, אם אינך זקוק לה עוד. יכולת של החלפה בשירות עצמי וביטול אינה זמינה ללקוחות של ההסכם הארגוני הממשלתי של ארה"ב. סוגי מנויים אחרים של ממשלת ארה"ב, כולל Pay-As-You-Go ו- CSP נתמכים. כדי לבצע החלפה או החזר כספי עבור הזמנה קיימת, נדרשת גישת בעלים בהזמנה.

השלבים הבאים מדריכים בהליך להשלמת העסקה

1.היכנס לפורטל [Azure שלך.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) בחר את ההזמנות שברצונך להחזיר ולחץ **על Exchange** 2.בחר את מוצר ה- VM שברצונך לרכוש והקלד כמות. ודא שסכום הרכישה החדש גדול מסכום ההחזרה [קבע את הגודל הנכון לפני הרכישה.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.סקור והשלם את העסקה

**החזר כספי עבור מופע שמור**

כדי להחזיר הזמנה, עבור אל **פרטי הזמנה** ולחץ על **החזר**

**החזר כספי מדורג:**

**Pro ההקצבה ודוגמאות הדרישה המינימלית עבור החזר והחלפה** דוגמה להזמנה מראש:

- רכשת RI לתקופת מנוי של שנה אחת ב- $120 ב- 1 בינואר
- ב- 7 באפריל אתה מעוניין להחזיר הזמנה זו או להחליף אותה
- מאחר שההזמנה היתה פעילה במשך 97 יום, תקבל החזר של (1-97/365) * 120 דולר. (כלומר, 88.1 דולר). בשלב זה אין קנס על החזרים כספיים
- אם אתה מחליף רכישה, הרכישה החדשה אמורה להיות גדולה מ- 88.1 דולר
- בשלב זה אין קנסות על החזרים כספיים

**דוגמה להזמנה בתוכנית חיוב:**

- רכשת RI לתקופת מנוי של שנה אחת ב- 10 דולר בחודש
- ב- 7 באפריל אתה מעוניין להחזיר הזמנה זו או להחליף אותה
- כיוון שהתשלום האחרון התרחש 7 ימים, תקבל החזר של (1-7/31) * 10 דולר. (כלומר, 7.74 דולר).
- התשלומים העתידיים שבוטלו הם $80. בשלב זה אין קנס על החזרים כספיים
- ביטול זה ינכה מההחזר בסך $87.74 ממגבלת ההחזר בסך $50,000
- אם אתה מחליף רכישה, הרכישה החדשה אמורה להיות גדולה מ- 87.74 דולר

**לא ניתן לראות חשבונית עבור תקופת החיוב האחרונה**

כמה סיבות אפשריות לכך שלא תראה חשבונית:

- יש לך סכום אשראי חודשי עם המנוי שלך שלא לחרוג או שיש לך גירסת ניסיון ללא תשלום. חשבונית נוצרת רק כאשר אתה חייב כסף
- עברו פחות מ- 30 יום מהיום שבו נרשמת כמנוי ל- Azure
- החשבונית עדיין לא נוצרה. המתן עד סוף תקופת החיוב
- אם אינך מנהל החשבון, ייתכן שחשבוניות ישנות יותר לא יהיו זמינות לך

**הורד את החשבונית שלך מ- Azure portal (.pdf)**

- בחר את המנוי שלך [מהדף מנויים](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) בפורטל Azure [כמשתמש בעל גישה לחשבוניות](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- בחר **חשבוניות**
- לחץ **על הורד חשבונית** כדי להציג עותק של חשבונית ה- PDF שלך. אם כתוב **"לא זמין",** ראה מדוע איני רואה [חשבונית עבור תקופת החיוב האחרונה?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**קבלת החשבונית בדואר אלקטרוני (.pdf)**

- בחר את המנוי שלך [מהדף מנויים.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) לחץ **על חשבוניות ולאחר מכן** שלח את החשבונית שלי בדואר אלקטרוני
- לחץ **על ההצטרפות** וקבל את התנאים. יהיה עליך להצטרף לכל מנוי בבעלותך

הערה: אם אינך מקבל הודעת דואר אלקטרוני לאחר ביצוע השלבים, ודא שכתובת הדואר האלקטרוני שלך נכונה [בהעדפות התקשורת בפרופיל שלך](https://account.windowsazure.com/profile)

**הורד את נתוני השימוש שלך בפורטל Azure**

- היכנס למרכז [החשבון של Azure כמנהל](https://account.windowsazure.com/Subscriptions) [החשבון](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- בחר את המנוי שעבורו ברצונך לקבל את פרטי החשבונית והשימוש
- בחר **היסטוריית חיובים**
- בחר **הצג משפט נוכחי** כדי לראות הערכה של החיובים שלך בעת יצירת ההערכה
- בחר **הורד שימוש** כדי להוריד את נתוני השימוש היומיים כקובץ CSV. אם אתה רואה שתי גירסאות זמינות, הורד את גירסה 2

שאלות נוספות: [בקר במסמכי מופע שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**מסמכים מומלצים**

- [יסודות החיוב](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת אופן ההחלה של הנחת מופע שמור](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הורדה או הצגה של חשבונית החיוב של Azure וניתוני שימוש יומיים](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת אופן ההחלה של הנחת מופע שמור](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת השימוש במופע שמור עבור מנוי Pay-As-You-Go שלך](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [הבנת השימוש במופע שמור עבור ההרשמה שלך לארגון](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows עלויות תוכנה אינן כלולות במופעים שמורים](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [מופעים שמורים בתוכנית שותפים ספק פתרונות ענן (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)