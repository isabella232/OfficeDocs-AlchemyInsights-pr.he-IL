---
title: מסירת דואר אלקטרוני באמצעות Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117984"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="21200-102">הגדרת התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="21200-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="21200-103">לקבלת מידע על האפשרויות העומדות בפניך והשלבים הדרושים, ראה [כיצד להגדיר התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני באמצעות Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="21200-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="21200-104">אם יש לך מכשיר או יישום שהפסקת לפעול לאחרונה, הבעיות הנפוצות ביותר הן:</span><span class="sxs-lookup"><span data-stu-id="21200-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="21200-105">**אימות שגיאות קשורות בעת שימוש בהגשת לקוח SMTP Auth** לאחרונה ביצענו כמה שינויים הקשורים לאימות SMTP.</span><span class="sxs-lookup"><span data-stu-id="21200-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="21200-106">לקבלת מידע נוסף אודות פתרון בעיות, עיין בסעיף האימות שלא נכשל בפתרון בעיות במדפסות, סורקים [ויישומים של LOB](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)ששולחים דואר אלקטרוני באמצעות Microsoft 365 או Office 365.</span><span class="sxs-lookup"><span data-stu-id="21200-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="21200-107">**אנו מקבלים רק את גירסת TLS 1.2 בעת יצירת חיבור מאובטח Office 365** אם אתה משתמש בחיבור מאובטח (TLS), ודא שהתקן היישום שלך תומך ב- TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="21200-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="21200-108">לקבלת מידע נוסף, ראה [הכנת TLS 1.2 ב- Office 365 ו- Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="21200-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="21200-109">לקבלת בעיות ופתרונות אחרים, ראה [פתרון בעיות במדפסות, סורקים](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)ויישומים של LOB ששולחים דואר אלקטרוני באמצעות Microsoft 365 או Office 365 .</span><span class="sxs-lookup"><span data-stu-id="21200-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="21200-110">כדי לראות את המכשירים המושפעים, עבור אל [דוח לקוחות אימות SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="21200-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="21200-111">**הערה:** Exchange Online אינו מתאים לתרחישי דיוור בצובר.</span><span class="sxs-lookup"><span data-stu-id="21200-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="21200-112">כדי לשלוח דואר אלקטרוני מסחרי בצובר (לדוגמה, ידיעונים של לקוחות), עליך להשתמש בספקים של ספקים חיצוני המתמחים בשירותים אלה.</span><span class="sxs-lookup"><span data-stu-id="21200-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
