---
title: 2491 הודעות דוא ל התראה מתוך ' Phish נמסר בשל מדיניות הדייר או המשתמש עקיפה '
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758929"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="0e29c-102">התראה הודעות דוא ל מתוך ' Phish נמסר בשל מדיניות הדייר או לעקוף את המשתמש</span><span class="sxs-lookup"><span data-stu-id="0e29c-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="0e29c-103">מדיניות התראה המהווה ברירת מחדל בשם "Phish נמסר עקב הדייר או עקיפת המשתמש" התגלגל החוצה לדיירים עם Office 365 ATP ו-P2 רשיונות.</span><span class="sxs-lookup"><span data-stu-id="0e29c-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="0e29c-104">אם קיבלת התראה זו, להלן השלבים לחקירת:</span><span class="sxs-lookup"><span data-stu-id="0e29c-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="0e29c-105">מתוך הודעת ההתראה, לחץ על **הצג התראה** כדי לעבור לעמוד ' **התראות** ' במרכז התאימות של אבטחה _ אמפר _.</span><span class="sxs-lookup"><span data-stu-id="0e29c-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="0e29c-106">בחר את ההתראה כדי לראות את האפשרות **להציג את רשימת ההודעות** או **להציג הודעות בסייר**.</span><span class="sxs-lookup"><span data-stu-id="0e29c-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="0e29c-107">שתי אפשרויות אלה מאפשרות לך לקבל את פרטי ההודעה, הכוללת את מזהה ההודעה.</span><span class="sxs-lookup"><span data-stu-id="0e29c-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="0e29c-108">שים לב שהקישור סייר האיומים יסנן באופן אוטומטי את ההודעות המתאימות לקריטריוני ההתראה.</span><span class="sxs-lookup"><span data-stu-id="0e29c-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="0e29c-109">ייתכן שיהיה עליך לכוונן את מסנן התאריכים בסייר האיומים.</span><span class="sxs-lookup"><span data-stu-id="0e29c-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="0e29c-110">הודעת הדיוג נמסרה עקב עקיפה שהוגדרה באופן ידני:</span><span class="sxs-lookup"><span data-stu-id="0e29c-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="0e29c-111">שולח או קבוצת מחשבים מותרים שהוגדרו על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="0e29c-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="0e29c-112">שולח או קבוצת מחשבים מותרים שהוגדרו על-ידי המנהל במדיניות נגד דואר זבל.</span><span class="sxs-lookup"><span data-stu-id="0e29c-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="0e29c-113">כתובת IP מותרת במדיניות של מסנן חיבורים.</span><span class="sxs-lookup"><span data-stu-id="0e29c-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="0e29c-114">כלל זרימת דואר (הידוע גם ככלל תעבורה) שתצורתו נקבעה לאפשר הודעות ב-.</span><span class="sxs-lookup"><span data-stu-id="0e29c-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="0e29c-115">אם אתה סבור שההודעה סומנה באופן שגוי כ-phish, השתמש [בתוספת הודעת הדוח](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) של Outlook כדי לשלוח דגימות של הודעות ל-Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e29c-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
