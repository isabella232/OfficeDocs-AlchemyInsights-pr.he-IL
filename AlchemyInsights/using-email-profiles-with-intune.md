---
title: שימוש בפרופילי דוא ל עם Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555255"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="94e72-102">שימוש בפרופילי דוא ל עם Intune</span><span class="sxs-lookup"><span data-stu-id="94e72-102">Using email profiles with Intune</span></span>

<span data-ttu-id="94e72-103">ניתן להשתמש בIntune כדי ליצור ולפרוס פרופילי דואר אלקטרוני עבור לקוח הדואר האלקטרוני יליד (מובנה) בפלטפורמות התקן מרובות.</span><span class="sxs-lookup"><span data-stu-id="94e72-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="94e72-104">לקבלת מידע אודות חלק מההגבלות המשויכות לפרופילי דואר אלקטרוני, כולל אופן הטיפול בפרופילים קיימים וכיצד להסיר פרופילי דואר אלקטרוני, ראה [הוספת הגדרות דואר אלקטרוני להתקנים באמצעות Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="94e72-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="94e72-105">לקבלת מידע נוסף על אופן יצירת פרופילי דואר אלקטרוני עבור כל פלטפורמת התקן, ראה:</span><span class="sxs-lookup"><span data-stu-id="94e72-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="94e72-106">הגדרות התקן אנדרואיד כדי לקבוע תצורה של דואר אלקטרוני, אימות וסנכרון בIntune</span><span class="sxs-lookup"><span data-stu-id="94e72-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="94e72-107">הוספת הגדרות דואר אלקטרוני עבור iOS והתקני iPadOS ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="94e72-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="94e72-108">הגדרות פרופיל דואר אלקטרוני ב-Microsoft Intune עבור התקנים המפעילים את Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="94e72-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="94e72-109">הגדרות פרופיל דואר אלקטרוני עבור התקנים שבהם פועל Windows 10 ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="94e72-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="94e72-110">**בעיית סינכרון משותפת**</span><span class="sxs-lookup"><span data-stu-id="94e72-110">**Common syncing issue**</span></span>

<span data-ttu-id="94e72-111">**נוקס על פרופיל דוא ל אנדרואיד מונע משתמשים אנשי קשר, לוח שנה, ומשימות, מלהיות מסונכרן להתקני משתמש.**</span><span class="sxs-lookup"><span data-stu-id="94e72-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="94e72-112">נוקס על דמוי אדם נוקס פרופיל דוא ל מציע למנהל את האפשרות להחליט אילו סוגי תוכן מסונכרנים למכשיר על ידי הגדרת כל אחד מאופשר.</span><span class="sxs-lookup"><span data-stu-id="94e72-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="94e72-113">אם ההגדרה עבור אחד מסוגי התוכן מוגדרת **כ'לא נקבעה** ' (ברירת המחדל), סוג תוכן זה אינו מסונכרן באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="94e72-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="94e72-114">משתמש עשוי לאפשר את סוג התוכן הרצוי ישירות על ההתקן באופן ידני, אך תצורה זו מוחלפת בהגדרת המדיניות Intune והסינכרון נפסק עבור סוג תוכן זה.</span><span class="sxs-lookup"><span data-stu-id="94e72-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

