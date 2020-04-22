---
title: 5.4.1 האנטי ספאם לתפוס-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707912"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="7fb0c-102">תקן בעיות מסירה עבור קוד שגיאה 550 5.4.1 ממסר גישה נדחתה</span><span class="sxs-lookup"><span data-stu-id="7fb0c-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="7fb0c-103">בעיה זו [מתרחשת בעת בדיקה כדי לבדוק אם כתובת דואר אלקטרוני היא חוקית כדי למנוע](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) הסגת זמן בעת הזנת הרשת של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7fb0c-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="7fb0c-104">נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="7fb0c-104">Try the following:</span></span>

1. <span data-ttu-id="7fb0c-105">קבע אם הבעיה היא ספציפית לתחום שלם או לכתובת דואר אלקטרוני יחידה:</span><span class="sxs-lookup"><span data-stu-id="7fb0c-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="7fb0c-106">כל התחום: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום כפנימי ולאחר מכן לחזור לסמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="7fb0c-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="7fb0c-107">כתובת דוא ל יחידה: לעתים יש לסנכרן את הכתובת; שינוי כתובת ה-proxy של smtp ולאחר מכן שינוי החזרה יכול לעזור.</span><span class="sxs-lookup"><span data-stu-id="7fb0c-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="7fb0c-108">קבע אם הבעיה היא ספציפית לקבוצה או לתיקיה ציבורית.</span><span class="sxs-lookup"><span data-stu-id="7fb0c-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="7fb0c-109">עבור סוגי אובייקטים מסוימים, ייתכן שיהיה צורך ליצור את האובייקטים באופן ידני באמצעות הספריה הפעילה.</span><span class="sxs-lookup"><span data-stu-id="7fb0c-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="7fb0c-110">אם אתה זקוק לעזרה נוספת, נא פתח כרטיס תמיכה וציין את היקף הבעיה (כולל סוג האובייקט שאתה שולח ל) כדי שנוכל לסייע לך בצורה טובה יותר.</span><span class="sxs-lookup"><span data-stu-id="7fb0c-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>