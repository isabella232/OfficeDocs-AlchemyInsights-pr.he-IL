---
title: פתרון בעיות אימות SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826416"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="9758c-102">פתרון בעיות אימות SMTP</span><span class="sxs-lookup"><span data-stu-id="9758c-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="9758c-103">אם אתה מקבל שגיאות 5.7.57 או 5.7.3 בעת ניסיון לשלוח דואר אלקטרוני מסוג SMTP ולאמת עם לקוח או יישום, עליך לבדוק כמה דברים:</span><span class="sxs-lookup"><span data-stu-id="9758c-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="9758c-104">ייתכן שהגשת SMTP מאומתת אינה זמינה דייר, או בתיבת הדואר שאתה מנסה להשתמש בה (בדוק את שתי ההגדרות).</span><span class="sxs-lookup"><span data-stu-id="9758c-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="9758c-105">כדי לקרוא עוד, ראה [הפיכת הגשת SMTP של לקוח מאומת לזמינה או ללא זמינה.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="9758c-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="9758c-106">בדוק אם [ברירות המחדל של Azure Security](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) זמינות עבור הדייר שלך; אם אפשרות זו זמינה, אימות SMTP באמצעות אימות בסיסי (המכונה גם מדור קודם; פעולה זו תשתמש בשם משתמש וסיסמה) תיכשל.</span><span class="sxs-lookup"><span data-stu-id="9758c-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
