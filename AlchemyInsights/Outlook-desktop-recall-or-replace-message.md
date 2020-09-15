---
title: שולחן העבודה של Outlook מאחזר או מחליף הודעת דואר אלקטרוני
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663991"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="dbd78-102">אחזור או החלפה של הודעת דואר אלקטרוני של Outlook</span><span class="sxs-lookup"><span data-stu-id="dbd78-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="dbd78-103">כמנהל המערכת, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="dbd78-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="dbd78-104">אין באפשרותך לאחזר הודעות ממרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="dbd78-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="dbd78-105">**באפשרותך לאחזר הודעות שנשלחות לאנשים בארגון שלך בלבד**.</span><span class="sxs-lookup"><span data-stu-id="dbd78-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="dbd78-106">אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אין באפשרותך לאחזר אותה.</span><span class="sxs-lookup"><span data-stu-id="dbd78-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="dbd78-107">באפשרותך **לאחזר הודעות שנשלחו מ-Outlook 2016 במחשב PC בלבד**.</span><span class="sxs-lookup"><span data-stu-id="dbd78-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="dbd78-108">אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותו.</span><span class="sxs-lookup"><span data-stu-id="dbd78-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="dbd78-109">כדי לאחזר או להחליף הודעת דואר אלקטרוני:</span><span class="sxs-lookup"><span data-stu-id="dbd78-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="dbd78-110">בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="dbd78-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="dbd78-111">לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.</span><span class="sxs-lookup"><span data-stu-id="dbd78-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="dbd78-112">בחר בכרטיסיה **הודעה** ולאחר מכן בחר באפשרות **פעולות**  >  **אחזור הודעה זו**.</span><span class="sxs-lookup"><span data-stu-id="dbd78-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="dbd78-113">בחר **באפשרות** **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף אותם בהודעה חדשה**ולאחר מכן בחר אישור.</span><span class="sxs-lookup"><span data-stu-id="dbd78-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="dbd78-114">אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.</span><span class="sxs-lookup"><span data-stu-id="dbd78-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="dbd78-115">ההצלחה או הכישלון של הודעת האחזור תלויים בהגדרות הנמען ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="dbd78-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="dbd78-116">לקבלת שלבים לבדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="dbd78-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="dbd78-117">חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך</span><span class="sxs-lookup"><span data-stu-id="dbd78-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="dbd78-118">אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לתפקיד ' ניהול חיפוש ' של גילוי אלקטרוני Manager או תאימות לחיפוש הודעות.</span><span class="sxs-lookup"><span data-stu-id="dbd78-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="dbd78-119">כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '.</span><span class="sxs-lookup"><span data-stu-id="dbd78-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="dbd78-120">הרשאות עבור תפקידים אלה מוקצות [במרכז האבטחה והתאימות](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="dbd78-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="dbd78-121">[צור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.</span><span class="sxs-lookup"><span data-stu-id="dbd78-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="dbd78-122">[התחבר אל מרכז האבטחה והתאימות של PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="dbd78-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="dbd78-123">אם אתה משתמש באימות רב-גורמי, ראה [התחברות למרכז האבטחה והתאימות של Microsoft 365 באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="dbd78-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>