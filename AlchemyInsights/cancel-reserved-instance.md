---
title: ביטול הזמנה
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807572"
---
# <a name="cancelling-reservation"></a>ביטול הזמנה

- **שירות עצמי:** באפשרותך לבטל או להחליף מופע שמור בעצמך באמצעות [הפורטל התכלת](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנה ולחץ על החזר או על exchange. שים לב שעליך להיות בעל גישה לבעלים בהזמנת ההזמנה כדי לבצע החלפה או החזר. גישה רק להזמנה לא תאפשר לך להמשיך בהחזר או ב-exchange. בקש מהבעלים של הזמנת ההזמנות להעניק לך גישה לבעלים להזמנת ההזמנה
- **מדיניות Exchange:** באפשרותך להחליף הזמנה להזמנה אחרת מאותו סוג – אין **קנסות** על חילופי הזמנות. המחויבות הכוללת של ההזמנה החדשה צריכה להיות גדולה יותר מהסכום של סכום ההחזר של ההזמנה שחלפה והתשלומים החודשיים העתידיים (אם ישים)
- **מדיניות החזר:** סכום ההחזר הכספי והתשלומים העתידיים שבוטלו אינם יכולים לחרוג מ-$50,000 USD בחלון מתגלגל של 12 חודשים. אנחנו **לא גובים כל עונש** על החזרים, אך הם יכולים לחייב אותו על החזרים עתידיים  
    **חריגים:** יכולת exchange וביטול של שירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני של ממשלת ארה"ב
- התמיכה ב- **API/PS/CLI** אינה זמינה לביטול ולזיכוי [של חילופים והחזרים בשירות עצמי עבור הזמנות של שירותים בתכלת](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- יכולת exchange וביטול של שירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני של ממשלת ארה"ב. סוגי מנויים אחרים של ממשלת ארצות הברית, כולל התמיכה בתשלום-לפי-לך ובCSP

[מידע נוסף: כיצד מעובדים הטרנזקציות return ו-exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
[מידע נוסף: מדיניות Exchange והחזר כספי](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
שאלות נוספות: [בקר במסמכי מופע שמורים](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**החלפת מופע שמור קיים (שירות עצמי)**

באפשרותך להחליף הזמנה להזמנה אחרת מאותו סוג. באפשרותך גם להחזיר הזמנה, עד $50,000 USD בשנה, אם אינך זקוק לה עוד. יכולת exchange וביטול של שירות עצמי אינה זמינה עבור לקוחות הסכם ארגוני של ממשלת ארה"ב. סוגי מנויים אחרים של ארצות הברית, כולל התמיכה בתשלום לפי-הנסיעה ו-CSP. עליך להיות בעל גישה לבעלים בהזמנת ההזמנה כדי להחליף או להחזיר הזמנה קיימת.

השלבים הבאים ינחו לגבי ההליך להשלמת הטרנזקציה

1. היכנס [לפורטל התכלת](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). בחר את ההזמנות שברצונך להחזיר ולחץ על **Exchange**
2. בחר את מוצר ה-VM שברצונך לרכוש והקלד כמות. ודא שסכום הרכישה החדש הוא יותר מסכום ההחזרה [הקובע את הגודל הנכון לפני הרכישה](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. סקירה והשלמה של הטרנזקציה

**החזר כספי עבור מופע שמור**

כדי להחזיר הזמנה, עבור אל **פרטי ההזמנה** ולחץ על **החזר כספי**

**החזר Pro-מדורג:**

**דוגמאות לדרישת מינימום ודרישות מינימום להחזר ולהחלפה**  
דוגמה להזמנה מראש:

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

**מסמכים מומלצים**

- [אופן העיבוד של טרנזקציות return ו-exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [מדיניות Exchange והחזר כספי](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)