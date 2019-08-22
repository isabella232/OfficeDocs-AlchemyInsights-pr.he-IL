---
title: יצירת פרופילים ומדיניות Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 11516232e7ad1fb1d54f07bccd31d586d5c04d42
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514764"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="2ccda-102">יצירת מדיניות Intune ופרופילים</span><span class="sxs-lookup"><span data-stu-id="2ccda-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="2ccda-103">Intune, תוכל ליצור מדיניות ופרופילים לעשות דברים אחרים.</span><span class="sxs-lookup"><span data-stu-id="2ccda-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="2ccda-104">**פרופילי הרשמה**: לקבוע מראש את תצורת ההתקנים שלך על-ידי הפלטפורמה, אפשר קירבה משתמש, השתמש אימות מגורמים רבים, ועוד.</span><span class="sxs-lookup"><span data-stu-id="2ccda-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="2ccda-105">[מהו התקן הרשמה](https://docs.microsoft.com/intune/device-enrollment), ליצור פרופילים הרשמה עבור [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), ו- [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) הן משאבים טובה.</span><span class="sxs-lookup"><span data-stu-id="2ccda-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="2ccda-106">**פריטי מדיניות של תאימות**: להגדיר כללים והגדרות המתבססות על התקנים חייב להיות תואם.</span><span class="sxs-lookup"><span data-stu-id="2ccda-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="2ccda-107">אתה יכול גם להשתמש בפריטי מדיניות של תאימות כדי לפקח על התקנים, וליידע את המשתמשים של אי-תאימות.</span><span class="sxs-lookup"><span data-stu-id="2ccda-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="2ccda-108">תחילת העבודה עם [מדיניות תאימות ההתקן](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="2ccda-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="2ccda-109">**פריטי מדיניות של גישה מותנית**: עזרה משאבים ארגונית מאובטחת, בהתאם לתנאים שאתה מזין.</span><span class="sxs-lookup"><span data-stu-id="2ccda-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="2ccda-110">לדוגמה, עבור התקנים שאינם תואמי, השתמש גישה מותנה כדי להגביל גישה אל דואר אלקטרוני ו- SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2ccda-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="2ccda-111">[מהי גישה מותנית](https://docs.microsoft.com/intune/conditional-access) [דרכים נפוצות לשימוש גישה מותנית](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) הם משאבים טוב כדי להתחיל.</span><span class="sxs-lookup"><span data-stu-id="2ccda-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="2ccda-112">**פרופילי תצורה**: ניהול תכונות והגדרות במכשירים, לרבות הגדרות דואר אלקטרוני, הוסף רשת WiFi, להשתמש תבניות מוכללות, תכונות של iOS בקרת התקן macOS ועוד.</span><span class="sxs-lookup"><span data-stu-id="2ccda-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="2ccda-113">להתחיל לעבוד בכל [הפרופילים תצורת ההתקן](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="2ccda-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="2ccda-114">קישורים שימושיים:</span><span class="sxs-lookup"><span data-stu-id="2ccda-114">Helpful links:</span></span>

- [<span data-ttu-id="2ccda-115">שאלות, בעיות נפוצות, ופתרונות עם פרופילי Intune ומדיניות של התקן</span><span class="sxs-lookup"><span data-stu-id="2ccda-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="2ccda-116">פתרון בעיות של פרופילי Intune ומדיניות</span><span class="sxs-lookup"><span data-stu-id="2ccda-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
