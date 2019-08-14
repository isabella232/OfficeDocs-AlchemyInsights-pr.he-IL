---
title: הודעות אימייל התראה 2491 מן המדיניות 'דרוס נמסרה Phish עקב דיירים או משתמש'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391308"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="b4822-102">הודעות דוא ל התראה מן המדיניות 'דרוס נמסרה Phish עקב דיירים או משתמש'</span><span class="sxs-lookup"><span data-stu-id="b4822-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="b4822-103">מדיניות התראה ברירת המחדל בשם "Delivered Phish עקב עקיפה דיירים או משתמש" הוחזרה כדי דיירים עם Office 365 ATP P1 ו- P2 רשיונות.</span><span class="sxs-lookup"><span data-stu-id="b4822-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="b4822-104">אם קיבלת התראה זו, להלן השלבים כדי לחקור:</span><span class="sxs-lookup"><span data-stu-id="b4822-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="b4822-105">מתוך הודעת ההתראה, לחץ על **הצג התראה** כדי לעבור לדף **התראות** ב & אבטחה מרכז תאימות.</span><span class="sxs-lookup"><span data-stu-id="b4822-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="b4822-106">בחר את ההתראה כדי לראות את האפשרות **הצג הודעה רשימה** או **הצגת הודעות ב- Explorer**.</span><span class="sxs-lookup"><span data-stu-id="b4822-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="b4822-107">שתי אפשרויות אלה יביאו אותך אל הפרטים של ההודעה, כולל מזהה ההודעה.</span><span class="sxs-lookup"><span data-stu-id="b4822-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="b4822-108">שים לב כי הקישור Explorer איום באופן אוטומטי לסנן את ההודעות התואמות לקריטריונים התראה.</span><span class="sxs-lookup"><span data-stu-id="b4822-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="b4822-109">ייתכן שיהיה עליך להתאים את המסנן תאריך בסייר איום.</span><span class="sxs-lookup"><span data-stu-id="b4822-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="b4822-110">הודעת הדיוג נמסרה עקב עקיפה שתצורתה נקבעה באופן ידני:</span><span class="sxs-lookup"><span data-stu-id="b4822-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="b4822-111">השולח המותר או תחום מוגדר על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="b4822-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="b4822-112">השולח המותר או תחום שקבע המנהל ב מדיניות נגד דואר זבל.</span><span class="sxs-lookup"><span data-stu-id="b4822-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="b4822-113">כתובת ה-IP המותרות במדיניות מסנן חיבור.</span><span class="sxs-lookup"><span data-stu-id="b4822-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="b4822-114">דואר זרימה כלל (המכונה גם כלל התעבורה) מוגדרת לאפשר הודעות ב-.</span><span class="sxs-lookup"><span data-stu-id="b4822-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="b4822-115">אם אתה סבור כי ההודעה סומנה באופן שגוי כ- phish, השתמש ב- Outlook [תוספת הודעת דוח](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) כדי לשלוח הודעה דוגמאות ל- Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b4822-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
