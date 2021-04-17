---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821412"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="9d284-102">פתרון בעיות במסירת דואר אלקטרוני עבור קוד שגיאה 5.7.23</span><span class="sxs-lookup"><span data-stu-id="9d284-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="9d284-103">אמת את רשומת ה- DNS של SPF עבור התחום שלך ב- SPF או בודק רשומות DNS הזמין לציבור באינטרנט.</span><span class="sxs-lookup"><span data-stu-id="9d284-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="9d284-104">ודא שההודעה היוצאת לא זוהתה כנת זבל על-ידי Microsoft וניתב דרך מאגר [מסירת סיכונים גבוהים](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="9d284-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="9d284-105">הודעות ב' מאגר מסירה בסיכון גבוה' לא יעברו בדיקת SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המשמש כיעד.</span><span class="sxs-lookup"><span data-stu-id="9d284-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="9d284-106">אם הבעיה נמשכת, ייתכן שתצטרך לפנות למנהל של מארח הדואר שאתה מנסה לשלוח לו דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="9d284-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="9d284-107">רשום לעצמך את השגיאה החיצונית המפורטת הזמינה בה הודעת ההקפצת.</span><span class="sxs-lookup"><span data-stu-id="9d284-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="9d284-108">ייתכן שהתמיכה של Microsoft לא תוכל לסייע עוד יותר.</span><span class="sxs-lookup"><span data-stu-id="9d284-108">Microsoft support may not be able to assist further.</span></span>
