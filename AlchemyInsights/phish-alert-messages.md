---
title: 2491 הודעות דואר אלקטרוני של התראה ממדיניות 'דיוג נמסר עקב דייר או עקיפת משתמש'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544579"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="afd7e-102">התראת הודעות דואר אלקטרוני ממדיניות 'דיוג נמסר עקב דייר או עקיפת משתמש'</span><span class="sxs-lookup"><span data-stu-id="afd7e-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="afd7e-103">מדיניות התראה המוגדרת כברירת מחדל בשם "Phish Delivered עקב דייר או עקיפת משתמש" הוגלתה לדיירים עם Microsoft Defender עבור רשיונות P1 ו- P2 של Microsoft Defender עבור Office 365 P1 ו- P2.</span><span class="sxs-lookup"><span data-stu-id="afd7e-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="afd7e-104">אם קיבלת התראה זו, להלן השלבים לתחקור:</span><span class="sxs-lookup"><span data-stu-id="afd7e-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="afd7e-105">מתוך הודעת ההתראה, לחץ **על הצג** התראה כדי **לעבור** לדף התראות במרכז האבטחה & תאימות.</span><span class="sxs-lookup"><span data-stu-id="afd7e-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="afd7e-106">בחר את ההתראה כדי לראות את האפשרות להציג **רשימת הודעות או** **להציג הודעות בסייר**.</span><span class="sxs-lookup"><span data-stu-id="afd7e-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="afd7e-107">שתי אפשרויות אלה לוקחות אותך לפרטי ההודעה, הכוללת את מזהה ההודעה.</span><span class="sxs-lookup"><span data-stu-id="afd7e-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="afd7e-108">שים לב שהקישור 'סייר איומים' ילסנן באופן אוטומטי את ההודעות התואמות לקריטריוני ההתראה.</span><span class="sxs-lookup"><span data-stu-id="afd7e-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="afd7e-109">ייתכן שיהיה עליך להתאים את מסנן התאריך בסייר האיומים.</span><span class="sxs-lookup"><span data-stu-id="afd7e-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="afd7e-110">הודעת דיוג נמסרה עקב עקיפה שתצורתה נקבעה באופן ידני:</span><span class="sxs-lookup"><span data-stu-id="afd7e-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="afd7e-111">שולח או תחום מותרים המוגדרים על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="afd7e-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="afd7e-112">שולח או תחום מותרים המוגדרים על-ידי מנהל המערכת במדיניות למניעת דואר זבל.</span><span class="sxs-lookup"><span data-stu-id="afd7e-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="afd7e-113">כתובת IP מותרת במדיניות מסנן חיבור.</span><span class="sxs-lookup"><span data-stu-id="afd7e-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="afd7e-114">כלל זרימת דואר (הידוע גם ככלל תעבורה) שתצורתו נקבעה לאפשר הודעות.</span><span class="sxs-lookup"><span data-stu-id="afd7e-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="afd7e-115">אם אתה סבור שההודעה סומנה באופן שגוי כ- phish, השתמש Outlook התוספת 'הודעת [דוח'](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) כדי לשלוח דוגמאות הודעה ל- Microsoft.</span><span class="sxs-lookup"><span data-stu-id="afd7e-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
