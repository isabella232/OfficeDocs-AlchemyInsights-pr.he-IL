---
title: ביטול הזמנה
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819693"
---
# <a name="cancelling-reservation"></a>ביטול הזמנה

- **שירות עצמי: באפשרותך** לבטל או להחליף מופע שמור בעצמך באמצעות [פורטל Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנה ולחץ על החזר כספי או על Exchange. שים לב: כדי לבצע החלפה או החזר כספי, נדרשת גישת בעלים בהזמנה. גישה להזמנה בלבד לא תאפשר לך להמשיך בהחזר כספי או בהחלפה. בקש מהבעלים של ההזמנה להעניק לך גישת בעלים להזמנה
- **מדיניות החלפה:** באפשרותך להחליף הזמנה עבור הזמנה אחרת מאותו סוג – **אין קנסות** על החלפת הזמנה. ההתחייבות הכוללת להזמנה חדשה צריכה להיות גדולה יותר מסכום ההחזר עבור החלפת הזמנה וסכום התשלומים החודשיים העתידיים (אם רלוונטי)
- **מדיניות החזרים:** סכום ההחזר והתשלומים העתידיים שבוטלו אינם יכולים לעלות על 50,000 דולר בחלון פריסה של 12 חודשים. אנו לא **גובים כרגע קנסות** שניתנו על החזרים, אך ייתכן שנגבה אותם על החזרים עתידיים  
    **חריגים:** יכולת של החלפה בשירות עצמי וביטול אינה זמינה ללקוחות של ההסכם הארגוני הממשלתי של ארה"ב
- **תמיכת API / PS / CLI** אינה זמינה לביטול והחזרים [החלפות בשירות עצמי והחזרים עבור הזמנות Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- יכולת של החלפה בשירות עצמי וביטול אינה זמינה ללקוחות של ההסכם הארגוני הממשלתי של ארה"ב. סוגי מנויים אחרים של ממשלת ארה"ב, כולל Pay-As-You-Go ו- CSP נתמכים

מידע נוסף: [עיבוד של עסקאות החזרה והחלפה](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
מידע נוסף: [מדיניות החלפה והחזרים כספיים](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
שאלות נוספות: [בקר במסמכי מופע שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**החלפת מופע שמור קיים (בשירות עצמי)**

באפשרותך להחליף הזמנה עבור הזמנה אחרת מאותו סוג. תוכל גם להחזיר תשלום על הזמנה, בסכום של 50,000 דולר לכל היותר בשנה, אם אינך זקוק לה עוד. יכולת של החלפה בשירות עצמי וביטול אינה זמינה ללקוחות של ההסכם הארגוני הממשלתי של ארה"ב. סוגי מנויים אחרים של ממשלת ארה"ב, כולל Pay-As-You-Go ו- CSP נתמכים. כדי לבצע החלפה או החזר כספי עבור הזמנה קיימת, נדרשת גישת בעלים בהזמנה.

השלבים הבאים מדריכים בהליך להשלמת העסקה

1. היכנס לחשבון שלך ב [פורטל Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנות שברצונך להחזיר ולאחר מכן לחץ על **החלפה**
2. בחר את מוצר המחשב הוירטואלי (VM) שברצונך לרכוש והזן סכום. ודא שסכום הרכישה החדשה גדול מהסכום ההחזר הכולל[קבע את הגודל הנכון לפני הרכישה](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. בדוק את העסקה והשלם אותה

**החזר כספי עבור מופע שמור**

כדי להחזיר הזמנה, עבור אל **פרטי הזמנה** ולחץ על **החזר**

**החזר כספי מדורג:**

**דוגמאות לדרישות יחסיות ודרישות מינימליות עבור החזר והחלפה**  
דוגמה להזמנה מראש:

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

**מסמכים מומלצים**

- [עיבוד של עסקאות החזרה והחלפה](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [מדיניות החלפה והחזרים כספיים](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)