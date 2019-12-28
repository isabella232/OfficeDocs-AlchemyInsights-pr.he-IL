---
title: שליחת הודעות מותאמות אישית עם Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886858"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="209c3-102">כיצד לשלוח הודעות מותאמות אישית למשתמשי iOS מנוהלים והתקנים אנדרואיד</span><span class="sxs-lookup"><span data-stu-id="209c3-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="209c3-103">הודעות מותאמות אישית עבור Intune מעובדות על-ידי יישום פורטל החברה בהתקן של משתמש.</span><span class="sxs-lookup"><span data-stu-id="209c3-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="209c3-104">לאחר מכן, האפליקציה יוצרת את הודעת הדחיפה על המכשיר.</span><span class="sxs-lookup"><span data-stu-id="209c3-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="209c3-105">להלן דרישות מוקדמות של התקנים כדי לתמוך בקבלת הודעות מותאמות אישית, ועבור היישום לאחר מכן ליצור את הודעת הדחיפה:</span><span class="sxs-lookup"><span data-stu-id="209c3-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="209c3-106">ההתקן חייב להתקין את יישום הפורטל של החברה.</span><span class="sxs-lookup"><span data-stu-id="209c3-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="209c3-107">ההתקן חייב לאפשר ליישום פורטל החברה לשלוח הודעות דחיפה.</span><span class="sxs-lookup"><span data-stu-id="209c3-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="209c3-108">כאשר האפליקציה מותקנת או מתעדכנת, היא תנחה את המשתמש להתיר הודעות.</span><span class="sxs-lookup"><span data-stu-id="209c3-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="209c3-109">התקנים אנדרואיד חייב להיות Google Play שירותי מותקן.</span><span class="sxs-lookup"><span data-stu-id="209c3-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="209c3-110">המכשיר חייב להיות רשום עם Intune.</span><span class="sxs-lookup"><span data-stu-id="209c3-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="209c3-111">לקבלת מידע נוסף כולל כיצד לשלוח הודעה, עיין [בתיעוד של התכונה](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="209c3-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
