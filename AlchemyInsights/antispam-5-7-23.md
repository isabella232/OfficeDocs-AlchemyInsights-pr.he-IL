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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506444"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="635f0-102">תקן בעיות משלוח דוא ל עבור קוד שגיאה 5.7.23</span><span class="sxs-lookup"><span data-stu-id="635f0-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="635f0-103">אמת את רשומת ה-SPF DNS עבור התחום שלך בבודק רשומות מסוג SPF או DNS זמין לציבור באינטרנט.</span><span class="sxs-lookup"><span data-stu-id="635f0-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="635f0-104">ודא שההודעה היוצאת לא זוהתה כהודעת זבל על-ידי Microsoft ונותבה באמצעות [מאגר המסירה לסיכון גבוה](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="635f0-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="635f0-105">הודעות במאגר האספקה של הסיכון הגבוה לא יעברו בדיקות SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המהווה יעד.</span><span class="sxs-lookup"><span data-stu-id="635f0-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="635f0-106">אם הבעיה נמשכת, ייתכן שיהיה עליך לפנות למנהל המארח של הדואר שאליו אתה מנסה לשלוח דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="635f0-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="635f0-107">רשום את השגיאה החיצונית המפורטת הזמינה בהודעת הניתור.</span><span class="sxs-lookup"><span data-stu-id="635f0-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="635f0-108">ייתכן שהתמיכה של Microsoft לא תוכל לסייע בהמשך.</span><span class="sxs-lookup"><span data-stu-id="635f0-108">Microsoft support may not be able to assist further.</span></span>
