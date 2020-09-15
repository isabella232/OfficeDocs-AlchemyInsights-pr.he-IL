---
title: 5.4.1 DBEB לתפוס את כל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717362"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="9a3e7-102">פתרון בעיות במסירה עבור קוד שגיאה 550 הגישה של 5.4.1 ממסר נדחתה</span><span class="sxs-lookup"><span data-stu-id="9a3e7-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="9a3e7-103">בעיה זו מתרחשת בעת [בדיקה אם כתובת דואר אלקטרוני חוקית כדי למנוע את bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) בעת הכניסה לרשת Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="9a3e7-104">נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="9a3e7-104">Try the following:</span></span>

1. <span data-ttu-id="9a3e7-105">קבע אם הבעיה ספציפית לתחום כולו או לכתובת דואר אלקטרוני אחת:</span><span class="sxs-lookup"><span data-stu-id="9a3e7-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="9a3e7-106">תחום כולו: לפעמים יש לסנכרן את התחום; נסה [להגדיר את התחום לפנימי ולאחר מכן לחזור לסמכותי](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="9a3e7-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="9a3e7-107">כתובת דואר אלקטרוני יחידה: לפעמים צריך לסנכרן את הכתובת; שינוי כתובת ה-proxy של smtp ולאחר מכן שינוי שלו בחזרה יכול לעזור.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="9a3e7-108">קביעה אם הבעיה ספציפית לקבוצה או לתיקיה ציבורית.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="9a3e7-109">עבור סוגי אובייקטים מסוימים, ייתכן שיהיה עליך ליצור את האובייקטים באופן ידני ב-תכלת Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="9a3e7-110">אם אתה זקוק לעזרה נוספת, פתח כרטיס תמיכה וציין את טווח הבעיה (כולל סוג האובייקט שאליו אתה שולח) כדי שנוכל לסייע לך בצורה טובה יותר.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>