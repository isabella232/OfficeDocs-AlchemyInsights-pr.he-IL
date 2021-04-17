---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821448"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="29822-102">פתרון בעיות מסירה עבור קוד שגיאה 550 5.4.1 ממסר Access נדחה</span><span class="sxs-lookup"><span data-stu-id="29822-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="29822-103">בעיה זו מתרחשת [בעת בדיקה אם כתובת דואר אלקטרוני חוקית כדי למנוע החזרים חוזרים](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) בעת הזנת רשת Microsoft.</span><span class="sxs-lookup"><span data-stu-id="29822-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="29822-104">נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="29822-104">Try the following:</span></span>

1. <span data-ttu-id="29822-105">קבע אם הבעיה ספציפית לתחום שלם או לכתובת דואר אלקטרוני בודדת:</span><span class="sxs-lookup"><span data-stu-id="29822-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="29822-106">התחום כולו: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום ל'פנימי' ולאחר מכן לחזור ל' סמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="29822-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="29822-107">כתובת דואר אלקטרוני בודדת: לפעמים יש לסנכרן את הכתובת; שינוי כתובת ה- Proxy של smtp ולאחר מכן שינוי כתובת ה- Proxy יכול לעזור.</span><span class="sxs-lookup"><span data-stu-id="29822-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="29822-108">קבע אם הבעיה ספציפית לקבוצה או לתיקיה ציבורית.</span><span class="sxs-lookup"><span data-stu-id="29822-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="29822-109">עבור סוגי אובייקטים מסוימים, ייתכן שיהיה צורך ליצור את האובייקטים באופן ידני ב- Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="29822-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="29822-110">אם אתה זקוק לעזרה נוספת, פתח כרטיס תמיכה וציין את היקף הבעיה (כולל סוג האובייקט שאתה שולח לו) כדי שנוכל לסייע לך טוב יותר.</span><span class="sxs-lookup"><span data-stu-id="29822-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>