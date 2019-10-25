---
title: אנטי ספאם-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682156"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="2cf6e-102">תקן בעיות משלוח דוא ל עבור קוד שגיאה 5.7.23</span><span class="sxs-lookup"><span data-stu-id="2cf6e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="2cf6e-103">אמת את רשומת ה-SPF DNS עבור התחום שלך בבודק רשומות מסוג SPF או DNS זמין לציבור באינטרנט.</span><span class="sxs-lookup"><span data-stu-id="2cf6e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="2cf6e-104">ודא שההודעה היוצאת לא זוהתה כהודעת זבל על-ידי Office 365 ונותבה דרך [מאגר האספקה הגבוה](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="2cf6e-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="2cf6e-105">הודעות במאגר האספקה של הסיכון הגבוה לא יעברו בדיקות SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המהווה יעד.</span><span class="sxs-lookup"><span data-stu-id="2cf6e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="2cf6e-106">אם הבעיה נמשכת, ייתכן שיהיה עליך לפנות למנהל המארח של הדואר שאליו אתה מנסה לשלוח דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="2cf6e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="2cf6e-107">רשום את השגיאה החיצונית המפורטת הזמינה בהודעת הניתור.</span><span class="sxs-lookup"><span data-stu-id="2cf6e-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="2cf6e-108">ייתכן שהתמיכה ב-Office 365 לא תוכל לסייע בהמשך.</span><span class="sxs-lookup"><span data-stu-id="2cf6e-108">Office 365 support may not be able to assist further.</span></span>