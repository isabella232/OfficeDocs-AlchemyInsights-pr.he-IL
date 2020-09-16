---
title: 2491 התראת דואר אלקטרוני של הודעות דואר אלקטרוני מ-' פיש נמסר עקב מדיניות של דייר או משתמש של עקיפת משתמשים
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728612"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="1873c-102">התרעת הודעות דואר אלקטרוני מ-' פיש נמסר עקב מדיניות של דייר או משתמש של עקיפת משתמשים</span><span class="sxs-lookup"><span data-stu-id="1873c-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="1873c-103">מדיניות התראה המוגדרת כברירת מחדל בשם "פיש נמסר בשל הדייר או הדריסה של המשתמש" הועברה לדיירים באמצעות רשיונות Office 365 ATP P1 ו-P2.</span><span class="sxs-lookup"><span data-stu-id="1873c-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="1873c-104">אם קיבלת התראה זו, להלן השלבים לחקירה:</span><span class="sxs-lookup"><span data-stu-id="1873c-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="1873c-105">מתוך הודעת ההתראה, לחץ על **הצג התראה** כדי לעבור לדף ' **התראות** ' במרכז התאימות של אבטחה &.</span><span class="sxs-lookup"><span data-stu-id="1873c-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="1873c-106">בחר את ההתראה כדי לראות את האפשרות **להצגת רשימת** הודעות או **להצגת הודעות בסייר**.</span><span class="sxs-lookup"><span data-stu-id="1873c-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="1873c-107">שתי אפשרויות אלה מעבירות אותך לפרטי ההודעה, הכוללת את מזהה ההודעה.</span><span class="sxs-lookup"><span data-stu-id="1873c-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="1873c-108">שים לב שהקישור של סייר האיומים מסנן באופן אוטומטי את ההודעות התואמות לקריטריוני ההתראה.</span><span class="sxs-lookup"><span data-stu-id="1873c-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="1873c-109">ייתכן שתצטרך להתאים את מסנן התאריכים בסייר האיומים.</span><span class="sxs-lookup"><span data-stu-id="1873c-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="1873c-110">הודעת הדיוג נמסרה עקב עקיפה שהוגדרה באופן ידני:</span><span class="sxs-lookup"><span data-stu-id="1873c-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="1873c-111">שולח או תחום מותר המוגדר על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1873c-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="1873c-112">שולח או תחום מותר המוגדר על-ידי מנהל המערכת במדיניות למניעת הודעות זבל.</span><span class="sxs-lookup"><span data-stu-id="1873c-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="1873c-113">כתובת IP מותרת במדיניות מסנן חיבורים.</span><span class="sxs-lookup"><span data-stu-id="1873c-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="1873c-114">כלל זרימת דואר (מכונה גם כלל תעבורה) שתצורתו נקבעה לאפשר הודעות ב-.</span><span class="sxs-lookup"><span data-stu-id="1873c-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="1873c-115">אם אתה סבור שההודעה סומנה באופן שגוי כ-פיש, השתמש [בתוספת הודעת הדוח](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) של Outlook כדי לשלוח דגימות הודעות ל-Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1873c-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
