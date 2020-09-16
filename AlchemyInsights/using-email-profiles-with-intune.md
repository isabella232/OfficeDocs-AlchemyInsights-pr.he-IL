---
title: שימוש בפרופילי דואר אלקטרוני עם כוונון
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653289"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="3d31e-102">שימוש בפרופילי דואר אלקטרוני עם כוונון</span><span class="sxs-lookup"><span data-stu-id="3d31e-102">Using email profiles with Intune</span></span>

<span data-ttu-id="3d31e-103">ניתן להשתמש ב-intune כדי ליצור ולפרוס פרופילי דואר אלקטרוני עבור לקוח הדואר האלקטרוני המוכלל (מוכלל) בפלטפורמות התקן מרובות.</span><span class="sxs-lookup"><span data-stu-id="3d31e-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="3d31e-104">לקבלת מידע אודות חלק מההגבלות המשויכות לפרופילי דואר אלקטרוני, כולל אופן הטיפול בנוכחות פרופילים קיימים וכיצד להסיר פרופילי דואר אלקטרוני, ראה [הוספת הגדרות דואר אלקטרוני למכשירים באמצעות ' שימוש בעידון](https://docs.microsoft.com/intune/email-settings-configure)'.</span><span class="sxs-lookup"><span data-stu-id="3d31e-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="3d31e-105">לקבלת מידע נוסף אודות אופן היצירה של פרופילי דואר אלקטרוני עבור כל פלטפורמת מכשיר, ראה:</span><span class="sxs-lookup"><span data-stu-id="3d31e-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="3d31e-106">הגדרות התקן של Android לקביעת תצורה של דואר אלקטרוני, אימות וסינכרון בתוך המנגינה</span><span class="sxs-lookup"><span data-stu-id="3d31e-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="3d31e-107">הוספת הגדרות דואר אלקטרוני עבור מכשירי iOS ו-iPadOS ב-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="3d31e-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="3d31e-108">הגדרות פרופיל דואר אלקטרוני ב-Microsoft intune עבור מכשירים שבהם פועל Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="3d31e-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="3d31e-109">הגדרות פרופיל דואר אלקטרוני עבור מכשירים שבהם פועל Windows 10 ב-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="3d31e-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="3d31e-110">**בעיית סינכרון נפוצה**</span><span class="sxs-lookup"><span data-stu-id="3d31e-110">**Common syncing issue**</span></span>

<span data-ttu-id="3d31e-111">**פרופיל הדואר האלקטרוני של נוקס ב-Android מונע מאנשי קשר, לוח שנה ומשימות של משתמשים, מלהיות מסתנכרן עם מכשירי משתמשים.**</span><span class="sxs-lookup"><span data-stu-id="3d31e-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="3d31e-112">פרופיל הדואר האלקטרוני של נוקס ב-Android נוקס מציע למנהל את האפשרות להחליט אילו סוגי תוכן מסונכרנים למכשיר על-ידי הגדרת כל אחד מהם לזמין.</span><span class="sxs-lookup"><span data-stu-id="3d31e-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="3d31e-113">אם ההגדרה עבור כל אחד מסוגי התוכן מוגדרת ל- **לא נקבעה תצורה** (ברירת המחדל), סוג תוכן זה אינו מסתנכרן באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="3d31e-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="3d31e-114">המשתמש עשוי להפוך את סוג התוכן לזמין ישירות במכשיר באופן ידני, אך תצורה זו מוחלפת על-ידי הגדרת המדיניות ' שינוי צורה ', והסינכרון מפסיק עבור סוג תוכן זה.</span><span class="sxs-lookup"><span data-stu-id="3d31e-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

