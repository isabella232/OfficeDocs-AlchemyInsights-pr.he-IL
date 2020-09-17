---
title: אירעה שגיאה בעת אימות שגיאת אסימון גישה במהלך ניתוח שולחן עבודה על הסיפון
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783552"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="098ed-102">השגיאה "אירעה שגיאה באימות אסימון גישה" במהלך ניתוח שולחן העבודה המשולב</span><span class="sxs-lookup"><span data-stu-id="098ed-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="098ed-103">שגיאה זו נצפתה בדרך כלל כאשר אסימון האימות פג.</span><span class="sxs-lookup"><span data-stu-id="098ed-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="098ed-104">בדרך כלל, רענון הדף מרענן את האסימון.</span><span class="sxs-lookup"><span data-stu-id="098ed-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="098ed-105">עם זאת, בעיה זו עשויה להימשך אם מדיניות גישה מותנית מוחלת על החשבון המשמש לניתוח שולחן העבודה בלוח.</span><span class="sxs-lookup"><span data-stu-id="098ed-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="098ed-106">באפשרותך לסקור את יומני הכניסה של תכלת לספירה בפורטל תכלת כדי לבדוק אם קיימות כשלונות כניסה עבור החשבון הנמצא בשימוש עבור ניתוח שולחן עבודה המשולב.</span><span class="sxs-lookup"><span data-stu-id="098ed-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="098ed-107">לקבלת מידע נוסף אודות גישה מותנית, בקר [בתכנון פריסת הגישה המותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="098ed-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>