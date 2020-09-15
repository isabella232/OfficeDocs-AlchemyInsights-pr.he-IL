---
title: ספאם-5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717326"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="3ec72-102">פתרון בעיות במסירת דואר אלקטרוני עבור קוד שגיאה 5.7.23</span><span class="sxs-lookup"><span data-stu-id="3ec72-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="3ec72-103">אמת את רשומת ה-SPF DNS עבור התחום שלך בבודק רשומות SPF או DNS הזמין באופן ציבורי באינטרנט.</span><span class="sxs-lookup"><span data-stu-id="3ec72-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="3ec72-104">ודא שההודעה היוצאת לא זוהתה כהודעת זבל על-ידי Microsoft והמנותבת באמצעות [בריכת המסירה הגבוהה לסיכון](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="3ec72-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="3ec72-105">הודעות בבריכת המסירה בסיכון גבוה לא יעברו בדיקות SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המשמש כיעד.</span><span class="sxs-lookup"><span data-stu-id="3ec72-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="3ec72-106">אם הבעיה נמשכת, ייתכן שיהיה עליך לפנות למנהל המארח של הדואר שאליו אתה מנסה לשלוח דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="3ec72-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="3ec72-107">רשום לעצמך את השגיאה החיצונית המפורטת הזמינה בהודעת הניתור.</span><span class="sxs-lookup"><span data-stu-id="3ec72-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="3ec72-108">ייתכן שהתמיכה של Microsoft לא תוכל לסייע עוד.</span><span class="sxs-lookup"><span data-stu-id="3ec72-108">Microsoft support may not be able to assist further.</span></span>
