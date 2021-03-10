---
title: פתרון בעיות באישורי חתימה של SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693422"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>פתרון בעיות באישורי חתימה של SAML

כדי לפתור את בעיית אישור החתימה של SAML, בצע את השלבים המומלצים הבאים:

1. בעת הוספת יישום ארגוני התומך ב-SSO, התכלת יפיק אישור שנקרא ' [אישור חתימה של SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)'. אישור זה מכיל תאריך תפוגה של 3 שנים. כדי לשנות את תאריך התפוגה של האישור, ראה [התאמה אישית של תאריך התפוגה של אישור האיחוד והעברתה לאישור חדש](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. האפשרות ' תכלת ' תשתמש באישור זה כדי להחתים את האסימונים של SAML המבוקשים על-ידי היישום ולשלוח אותו ליישום עבור SSO מוצלח. כדי להשלים זאת, הורד את האישור מפורטל התכלת ושלח אותו לספק היישומים כדי להשלים את תהליך ה-SSO.

לאחר השלמת תהליך זה, היישום יאפשר לך לתת אמון באישור זה וכל האסימונים של SAML שנחתמו על-ידי אישור זה יתקבלו על-ידי היישום.

3. אם תוקף אישור זה פג, צור אישור חדש, עדכן אותו לספק היישומים ולאחר מכן הפוך אותו לפעיל בצד התכלת. לקבלת מידע נוסף, ראה [חידוש אישור שיפוג בקרוב](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> אם פג תוקפו של האישור, המשתמש לא נחסם.

4. [הוסף כתובת דואר אלקטרוני לקבלת הודעות](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) שיתקבלו לפני שפג תוקפו של האישור הנוכחי.

> [!NOTE]
> שלב 4 הוא אופציונלי.

5. שינוי אפשרויות חתימת האישורים של SAML והאלגוריתם לחתימת אישור. לקבלת מידע נוסף, ראה [שינוי אפשרויות חתימת אישורים והוספת אלגוריתם חתימה](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

