---
title: מסירת דואר אלקטרוני באמצעות Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023460"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="72fb1-102">הגדרת התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="72fb1-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="72fb1-103">לקבלת מידע על האפשרויות העומדות בפניך והשלבים הדרושים, ראה [כיצד להגדיר התקן רב-תכליתי או יישום לשליחת דואר אלקטרוני באמצעות Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="72fb1-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="72fb1-104">**הערה:** אם יש לך התקן או יישום שהפסיק לפעול לאחרונה, שים לב שהתחלנו לאחרונה [להפוך את הצופן של 3DES ללא זמין](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) בהתאם לתוכנית.</span><span class="sxs-lookup"><span data-stu-id="72fb1-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="72fb1-105">כדי לראות את המכשירים המושפעים, עבור אל [דוח לקוחות אימות SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="72fb1-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="72fb1-106">בין השגיאות הנפוצות: "כשל/שגיאה באימות", "כשל/שגיאה ב- TLS", "שגיאת אלגוריתם צופן", "חוסר התאמה באלגוריתם" או "החיבור התנתק".</span><span class="sxs-lookup"><span data-stu-id="72fb1-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="72fb1-107">כדי לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="72fb1-107">To resolve the issue:</span></span>

 - <span data-ttu-id="72fb1-108">**Windows Server 2003 עם IIS SMTP לא יפעל עוד – יש צורך בגירסה חדשה יותר של Windows.**</span><span class="sxs-lookup"><span data-stu-id="72fb1-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="72fb1-109">פנה לספק של היישום או ההתקן כדי לבדוק אם יש תמיכה בצופן מודרני או אם קיים עדכון.</span><span class="sxs-lookup"><span data-stu-id="72fb1-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
