---
title: שליחת הודעות מותאמות אישית עם Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992314"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="2a595-102">כיצד לשלוח הודעות מותאמות אישית למשתמשי iOS מנוהלים והתקנים אנדרואיד</span><span class="sxs-lookup"><span data-stu-id="2a595-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="2a595-103">הודעות מותאמות אישית עבור Intune מעובדות על-ידי יישום פורטל החברה בהתקן של משתמש.</span><span class="sxs-lookup"><span data-stu-id="2a595-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="2a595-104">לאחר מכן, האפליקציה יוצרת את הודעת הדחיפה על המכשיר.</span><span class="sxs-lookup"><span data-stu-id="2a595-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="2a595-105">להלן דרישות מוקדמות של התקנים כדי לתמוך בקבלת הודעות מותאמות אישית, ועבור היישום לאחר מכן ליצור את הודעת הדחיפה:</span><span class="sxs-lookup"><span data-stu-id="2a595-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="2a595-106">ההתקן חייב להתקין את יישום הפורטל של החברה.</span><span class="sxs-lookup"><span data-stu-id="2a595-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="2a595-107">ההתקן חייב לאפשר ליישום פורטל החברה לשלוח הודעות דחיפה.</span><span class="sxs-lookup"><span data-stu-id="2a595-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="2a595-108">כאשר האפליקציה מותקנת או מתעדכנת, היא תנחה את המשתמש להתיר הודעות.</span><span class="sxs-lookup"><span data-stu-id="2a595-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="2a595-109">התקנים אנדרואיד חייב להיות Google Play שירותי מותקן.</span><span class="sxs-lookup"><span data-stu-id="2a595-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="2a595-110">המכשיר חייב להיות רשום עם Intune.</span><span class="sxs-lookup"><span data-stu-id="2a595-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="2a595-111">לקבלת מידע נוסף כולל כיצד לשלוח הודעה, עיין [בתיעוד של התכונה](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="2a595-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
