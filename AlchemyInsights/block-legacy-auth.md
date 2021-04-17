---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820179"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="97c3b-102">חסימת אימות מדור קודם</span><span class="sxs-lookup"><span data-stu-id="97c3b-102">Blocking legacy authentication</span></span>

<span data-ttu-id="97c3b-103">אימות מדור קודם הוא מונח המפנה לבקשת אימות שהתבקשה על-ידי:</span><span class="sxs-lookup"><span data-stu-id="97c3b-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="97c3b-104">לקוחות Office ישנים יותר שלא משתמשים באימות מודרני (לדוגמה, לקוח Office 2010).</span><span class="sxs-lookup"><span data-stu-id="97c3b-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="97c3b-105">כל לקוח שמשתמש בפרוטוקולי דואר מדור קודם כגון IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="97c3b-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="97c3b-106">לקבלת מידע נוסף אודות חסימת אימות מדור קודם והפעלת אימות מודרני, עיין [בחסימת אימות מדור קודם](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="97c3b-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="97c3b-107">ברירות מחדל של אבטחה ב- Azure Active Directory (Azure AD) מקלות עליך להיות מאובטח ולעזור להגן על הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="97c3b-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="97c3b-108">ברירות מחדל של אבטחה מכילות הגדרות אבטחה מוגדרות מראש עבור התקפות נפוצות.</span><span class="sxs-lookup"><span data-stu-id="97c3b-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="97c3b-109">לקבלת מידע נוסף אודות ברירות מחדל של אבטחה, ראה [אילו ברירות מחדל של אבטחה?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="97c3b-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="97c3b-110">**הערה:** אם הדייר שלך נוצר ב- 22 באוקטובר 2019 או לאחר מכן, ייתכן שאתה חווה את אופן הפעולה החדש של secure-by-default וכבר יש לך ברירות מחדל של אבטחה זמינות בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="97c3b-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="97c3b-111">במאמץ להגן על כל המשתמשים שלנו, ברירות המחדל של האבטחה מוגלות לכל הדיירים החדשים שנוצרו.</span><span class="sxs-lookup"><span data-stu-id="97c3b-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
