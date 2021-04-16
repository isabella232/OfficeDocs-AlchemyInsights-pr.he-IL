---
title: אירעה שגיאה בעת אימות שגיאת אסימון גישה במהלך ניתוח שולחן העבודה בעת העלייה למטוס
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813689"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="29ae0-102">שגיאת "אירעה שגיאה בעת אימות אסימון גישה" במהלך ההסתה ל- Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="29ae0-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="29ae0-103">שגיאה זו נצפתה בדרך כלל כאשר פג תוקפו של אסימון האימות.</span><span class="sxs-lookup"><span data-stu-id="29ae0-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="29ae0-104">בדרך כלל, רענון הדף מרענן את האסימון.</span><span class="sxs-lookup"><span data-stu-id="29ae0-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="29ae0-105">עם זאת, בעיה זו עשויה לפתור אם חלה מדיניות Access מותנית כלשהי שחלה על החשבון המשמש לניתוח שולחני על הלוח.</span><span class="sxs-lookup"><span data-stu-id="29ae0-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="29ae0-106">באפשרותך לסקור את יומני הרישום של Azure AD Sign In בפורטל Azure כדי לראות אם זמינים כשלים בכניסה עבור החשבון המשמש עבור הכניסה ל- Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="29ae0-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="29ae0-107">לקבלת מידע נוסף אודות תות Access, בקר ב [תכנון פריסת Access מותן](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="29ae0-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>