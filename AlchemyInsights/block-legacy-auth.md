---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685599"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="c6e4a-102">חסימת אימות מדור קודם</span><span class="sxs-lookup"><span data-stu-id="c6e4a-102">Blocking legacy authentication</span></span>

<span data-ttu-id="c6e4a-103">אימות מדור קודם הוא מונח המפנה לבקשת אימות שבוצעה על-ידי:</span><span class="sxs-lookup"><span data-stu-id="c6e4a-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="c6e4a-104">לקוחות Office ישנים יותר שאינם משתמשים באימות מודרני (לדוגמה, לקוח Office 2010).</span><span class="sxs-lookup"><span data-stu-id="c6e4a-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="c6e4a-105">כל לקוח המשתמש בפרוטוקולי דואר מדור קודם כגון IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="c6e4a-106">לקבלת מידע נוסף אודות חסימת אימות מדור קודם והפיכת אימות מודרני לזמינה, ראה [חסימת אימות מדור קודם](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="c6e4a-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="c6e4a-107">ברירות מחדל של אבטחה ב-תכלת Active Directory (תכלת לספירה) מאפשרות לך להיות מאובטח יותר ולסייע בהגנה על הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="c6e4a-108">ברירות מחדל של אבטחה מכילות הגדרות אבטחה מוגדרות מוגדרות להתקפות נפוצות.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="c6e4a-109">לקבלת מידע נוסף אודות ברירות מחדל של אבטחה, עיין במאמר [מה הם ברירות מחדל של אבטחה?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="c6e4a-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="c6e4a-110">**הערה**: אם הדייר שלך נוצר ב-22 באוקטובר או אחרי ה-22 באוקטובר, 2019, ייתכן שאתה נתקל בהתנהגות המאובטחת החדשה המאובטחת כברירת מחדל ושכבר קיימות ברירות מחדל של אבטחה הזמינות בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="c6e4a-111">בניסיון להגן על כל המשתמשים שלנו, ברירות המחדל של האבטחה מסוכמות לכל הדיירים החדשים שנוצרו.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
