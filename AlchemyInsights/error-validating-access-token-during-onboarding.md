---
title: אירעה שגיאה בעת אימות שגיאת אסימון גישה במהלך ניתוח שולחן עבודה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741190"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="9570e-102">"אירעה שגיאה באימות אסימון גישה" במהלך ניתוח שולחני בעת העלייה למטוס</span><span class="sxs-lookup"><span data-stu-id="9570e-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="9570e-103">שגיאה זו נצפתה בדרך כלל כאשר פג תוקפו של אסימון האימות.</span><span class="sxs-lookup"><span data-stu-id="9570e-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="9570e-104">בדרך כלל, רענון הדף מרענן את האסימון.</span><span class="sxs-lookup"><span data-stu-id="9570e-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="9570e-105">עם זאת, בעיה זו יכולה להימשך אם יש פריטי מדיניות של גישה מותנית שהוחלו על החשבון המשמש לניתוח שולחן עבודה על הלוח.</span><span class="sxs-lookup"><span data-stu-id="9570e-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="9570e-106">באפשרותך לסקור את כניסת הכניסה למטה בתוך הפורטל כדי לבדוק אם קיימים כשלים כניסה עבור החשבון המשמש לניתוח שולחני בעת העלייה למטוס.</span><span class="sxs-lookup"><span data-stu-id="9570e-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="9570e-107">לקבלת מידע נוסף אודות גישה מותנית, בקר [בתוכנית הפריסה של גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="9570e-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>