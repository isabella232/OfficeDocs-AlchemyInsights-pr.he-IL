---
title: האחזור בשולחן העבודה של outlook או החלפה הודעת דואר אלקטרוני
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496112"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="f5257-102">אחזור או החלפה של הודעת דואר אלקטרוני של Outlook</span><span class="sxs-lookup"><span data-stu-id="f5257-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="f5257-103">כמנהל מערכת, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="f5257-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="f5257-104">אין אפשרות לאחזר הודעות ממרכז admin.</span><span class="sxs-lookup"><span data-stu-id="f5257-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="f5257-105">באפשרותך **רק הודעות האחזור אשר נשלחות לאנשים בארגון שלך**.</span><span class="sxs-lookup"><span data-stu-id="f5257-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="f5257-106">אם ההודעה נשלחה לכתובת Gmail, לדוגמה, אתה זוכר אותו.</span><span class="sxs-lookup"><span data-stu-id="f5257-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="f5257-107">באפשרותך **רק הודעות האחזור שנשלחו מ- Outlook 2016 במחשב**.</span><span class="sxs-lookup"><span data-stu-id="f5257-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="f5257-108">אם משתמש שולח הודעה באמצעות Outlook עבור Mac או ב- Outlook באינטרנט, אין אפשרות לאחזר אותה.</span><span class="sxs-lookup"><span data-stu-id="f5257-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="f5257-109">אחזור או החלפה של הודעת דואר אלקטרוני:</span><span class="sxs-lookup"><span data-stu-id="f5257-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="f5257-110">בחלונית התיקיות בצד ימין של חלון Outlook, בחר את התיקיה פריטים שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="f5257-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="f5257-111">לחץ פעמיים על ההודעה שברצונך לאחזר כדי לפתוח אותה.</span><span class="sxs-lookup"><span data-stu-id="f5257-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="f5257-112">בחר את הכרטיסיה **הודעה** ולאחר מכן בחר **פעולות** > **אחזור הודעה זו**.</span><span class="sxs-lookup"><span data-stu-id="f5257-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="f5257-113">בחר **למחוק עותקים שלא נקראו של הודעה זו** או **למחוק עותקים שלא נקראו ולהחליף בהודעה חדשה**, ולאחר מכן בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="f5257-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="f5257-114">אם אתה שולח הודעה חלופי, חבר את ההודעה ולאחר מכן בחר **לשלוח**.</span><span class="sxs-lookup"><span data-stu-id="f5257-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="f5257-115">ההצלחה או הכשלון של אחזור הודעה תלוי בהגדרות של הנמען ב- Outlook.</span><span class="sxs-lookup"><span data-stu-id="f5257-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="f5257-116">עבור השלבים לבדיקת האחזור, עיין [במאמר זה](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="f5257-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="f5257-117">חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון שלך</span><span class="sxs-lookup"><span data-stu-id="f5257-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="f5257-118">אם אינך מנהל כללי, יש להוסיף את החשבון שלך תפקיד מנהל גילוי אלקטרוני או תפקיד ניהול תאימות חיפוש כדי לחפש הודעות.</span><span class="sxs-lookup"><span data-stu-id="f5257-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="f5257-119">כדי למחוק הודעות, תצטרך להצטרף לקבוצה תפקיד ניהול הארגון או תפקיד ניהול חיפוש ומחק לצמיתות.</span><span class="sxs-lookup"><span data-stu-id="f5257-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="f5257-120">הרשאות עבור תפקידים אלה מוקצות ב [מרכז האבטחה והתאימות](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="f5257-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="f5257-121">[צור תוכן החיפוש](https://docs.microsoft.com/office365/securitycompliance/content-search) כדי למצוא את ההודעה כדי למחוק.</span><span class="sxs-lookup"><span data-stu-id="f5257-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="f5257-122">[להתחבר PowerShell מרכז תאימות ואבטחה](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="f5257-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="f5257-123">אם אתה משתמש אימות מגורמים רבים, ראה [התחברות אל Office 365 אבטחה ו- PowerShell מרכז תאימות באמצעות אימות מגורמים רבים](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="f5257-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>