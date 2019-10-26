---
title: שולחן העבודה של Outlook מאחזר או מחליף הודעת דואר אלקטרוני
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496112"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="0cb4b-102">אחזור או החלפה של הודעת דואר אלקטרוני של Outlook</span><span class="sxs-lookup"><span data-stu-id="0cb4b-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="0cb4b-103">כמנהל, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="0cb4b-104">אין באפשרותך לאחזר הודעות ממרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="0cb4b-105">**באפשרותך לאחזר הודעות שנשלחות לאנשים בארגונך בלבד**.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="0cb4b-106">אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אינך יכול לאחזר אותה.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="0cb4b-107">אתה יכול **רק לאחזר הודעות שנשלחו מ-Outlook 2016 במחשב**.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="0cb4b-108">אם משתמש שולח הודעה באמצעות Outlook for Mac או Outlook באינטרנט, אינך יכול לאחזר אותו.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="0cb4b-109">כדי לאחזר או להחליף הודעת דואר אלקטרוני:</span><span class="sxs-lookup"><span data-stu-id="0cb4b-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="0cb4b-110">בחלונית התיקיות שמשמאל לחלון Outlook, בחר את התיקיה פריטים שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="0cb4b-111">לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="0cb4b-112">בחר בכרטיסיה **הודעה** ולאחר מכן בחר **בפעולות** > **אחזור הודעה זו**.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="0cb4b-113">בחר באפשרות **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף בהודעה חדשה**ולאחר מכן בחר **באפשרות אישור**.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="0cb4b-114">אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **בשלח**.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="0cb4b-115">ההצלחה או הכישלון של אחזור הודעה תלויים בהגדרות הנמען ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="0cb4b-116">לקבלת שלבים לבדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="0cb4b-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="0cb4b-117">חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך</span><span class="sxs-lookup"><span data-stu-id="0cb4b-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="0cb4b-118">אם אינך מנהל כללי, יש להוסיף את חשבונך לתפקיד ניהול התפקיד של מנהל eDiscovery או חיפוש תאימות כדי לחפש הודעות.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="0cb4b-119">כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="0cb4b-120">הרשאות עבור תפקידים אלה מוקצות [במרכז האבטחה והתאימות](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="0cb4b-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="0cb4b-121">[יצור חיפוש תוכן](https://docs.microsoft.com/office365/securitycompliance/content-search) כדי למצוא את ההודעה שיש למחוק.</span><span class="sxs-lookup"><span data-stu-id="0cb4b-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="0cb4b-122">[התחבר למרכז האבטחה והתאימות PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0cb4b-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="0cb4b-123">אם אתה משתמש באימות מרובה גורמים, ראה [התחברות למרכז האבטחה והתאימות של Office 365 PowerShell באמצעות אימות מרובה גורמים](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0cb4b-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>