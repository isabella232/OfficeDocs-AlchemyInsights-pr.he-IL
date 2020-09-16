---
title: שליחת הודעות מותאמות אישית באמצעות כוונון
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720647"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="b3e96-102">כיצד לשלוח הודעות מותאמות אישית למשתמשים של מכשירי iOS ומכשירי Android מנוהלים</span><span class="sxs-lookup"><span data-stu-id="b3e96-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="b3e96-103">הודעות מותאמות אישית עבור ' שלחן ' מעובדות על-ידי האפליקציה ' פורטל החברה ' במכשיר של משתמש.</span><span class="sxs-lookup"><span data-stu-id="b3e96-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="b3e96-104">לאחר מכן האפליקציה יוצרת את ההודעה דחיפה במכשיר זה.</span><span class="sxs-lookup"><span data-stu-id="b3e96-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="b3e96-105">להלן דרישות מוקדמות של התקן כדי לתמוך בקבלת הודעות מותאמות אישית, ולאחר מכן כדי ליצור את הודעת הדחיפה:</span><span class="sxs-lookup"><span data-stu-id="b3e96-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="b3e96-106">היישום ' פורטל החברה ' חייב להיות מותקן במכשיר.</span><span class="sxs-lookup"><span data-stu-id="b3e96-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="b3e96-107">המכשיר חייב לאפשר לאפליקציית הפורטל של החברה לשלוח הודעות דחיפה.</span><span class="sxs-lookup"><span data-stu-id="b3e96-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="b3e96-108">כאשר האפליקציה מותקנת או מעודכנת, היא תנחה את המשתמש להתיר הודעות.</span><span class="sxs-lookup"><span data-stu-id="b3e96-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="b3e96-109">מכשירי Android חייבים להיות מותקנים ב-Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="b3e96-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="b3e96-110">יש לרשום את המכשיר באמצעות ' שלחן '.</span><span class="sxs-lookup"><span data-stu-id="b3e96-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="b3e96-111">לקבלת מידע נוסף, כולל כיצד לשלוח הודעה, עיין [בתיעוד התכונות](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="b3e96-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
