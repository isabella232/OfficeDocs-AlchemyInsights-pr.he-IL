---
title: הגדר תשובות אוטומטיות עבור תיבת דואר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509495"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="fad59-102">הגדר תשובות אוטומטיות עבור תיבת דואר של משתמש</span><span class="sxs-lookup"><span data-stu-id="fad59-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="fad59-103">**שיטה 1**</span><span class="sxs-lookup"><span data-stu-id="fad59-103">**Method 1**</span></span>

1. <span data-ttu-id="fad59-104">היכנס לפורטל של Office 365.</span><span class="sxs-lookup"><span data-stu-id="fad59-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="fad59-105">עבור אל **משתמשים > משתמשים פעילים** (או **קבוצות > תיבות דואר משותפות** אם תגדיר זאת בתיבת דואר משותפת).</span><span class="sxs-lookup"><span data-stu-id="fad59-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="fad59-106">בחר משתמש בעל תיבת דואר של Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="fad59-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="fad59-107">בתפריט הנפתח משמאל, עבור אל \*\*הגדרות דואר > תשובה אוטומטית (אם מדובר בתיבת דואר משותפת, פשוט לחץ על תשובות אוטומטיות במעוף החוצה).</span><span class="sxs-lookup"><span data-stu-id="fad59-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="fad59-108">**שיטה 2**</span><span class="sxs-lookup"><span data-stu-id="fad59-108">**Method 2**</span></span>

1. <span data-ttu-id="fad59-109">היכנס לפורטל הניהול של Office 365 באמצעות אישורי מנהל המערכת.</span><span class="sxs-lookup"><span data-stu-id="fad59-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="fad59-110">הרחב את **מרכזי הניהול**, ולאחר מכן לחץ על **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="fad59-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="fad59-111">לחץ על התמונה בפינה העליונה שמאלית, לחץ על **משתמש אחר** ולאחר מכן בחר את תיבת הדואר של המשתמש שברצונך לשנות.</span><span class="sxs-lookup"><span data-stu-id="fad59-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="fad59-112">בצד ימין, בחר **אפשרויות**, לחץ על **ארגן את הדואר האלקטרוני**, ולאחר מכן לחץ **תשובות אוטומטיות.**</span><span class="sxs-lookup"><span data-stu-id="fad59-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="fad59-113">**שיטה 3**</span><span class="sxs-lookup"><span data-stu-id="fad59-113">**Method 3**</span></span>

<span data-ttu-id="fad59-114">הפעל את ה- cmdlet הבא ב- Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="fad59-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="fad59-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="fad59-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="fad59-116">לקבל מידע נוסף אודות cmdlet זה, ראה [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="fad59-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
