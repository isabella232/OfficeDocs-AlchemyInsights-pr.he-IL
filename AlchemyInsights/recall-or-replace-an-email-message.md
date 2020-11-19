---
title: אחזור או החלפה של הודעת דואר אלקטרוני
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353507"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="6345f-102">אחזור או החלפה של הודעת דואר אלקטרוני ב-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6345f-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="6345f-103">**באפשרותך לאחזר הודעות שנשלחות לאנשים בארגון שלך בלבד**.</span><span class="sxs-lookup"><span data-stu-id="6345f-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="6345f-104">לדוגמה, אם ההודעה נשלחה לכתובת Gmail, אין באפשרותך לאחזר אותה.</span><span class="sxs-lookup"><span data-stu-id="6345f-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="6345f-105">באפשרותך **לאחזר רק הודעות שנשלחו מ-Outlook עבור המחשב**.</span><span class="sxs-lookup"><span data-stu-id="6345f-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="6345f-106">אם משתמש שולח הודעה באמצעות Outlook עבור Mac או Outlook באינטרנט, לא ניתן לאחזר אותו.</span><span class="sxs-lookup"><span data-stu-id="6345f-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="6345f-107">כמנהל דיירים, באפשרותך **לאחזר הודעות בשם משתמשים באמצעות PowerShell** (לקבלת מידע נוסף, ראה: [חיפוש ומחיקה של הודעות דואר אלקטרוני](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="6345f-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="6345f-108">אין באפשרותך לאחזר הודעות ממרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="6345f-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="6345f-109">גלול מטה אל "חיפוש ומחיקה של הודעות דואר אלקטרוני בארגון" לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="6345f-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="6345f-110">**אחזור או החלפה של הודעת דואר אלקטרוני ששלחת**</span><span class="sxs-lookup"><span data-stu-id="6345f-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="6345f-111">בחלונית התיקיות מימין לחלון Outlook, בחר את התיקיה פריטים שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="6345f-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="6345f-112">פתח את ההודעה שברצונך לאחזר.</span><span class="sxs-lookup"><span data-stu-id="6345f-112">Open the message that you want to recall.</span></span> <span data-ttu-id="6345f-113">עליך ללחוץ פעמיים כדי לפתוח את ההודעה.</span><span class="sxs-lookup"><span data-stu-id="6345f-113">You must double-click to open the message.</span></span> <span data-ttu-id="6345f-114">בחירת ההודעה כך שתופיע בחלונית הקריאה לא תאפשר לך לאחזר את ההודעה.</span><span class="sxs-lookup"><span data-stu-id="6345f-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="6345f-115">בכרטיסיה הודעה, בחר **פעולות**  >  **אחזור הודעה זו**.</span><span class="sxs-lookup"><span data-stu-id="6345f-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="6345f-116">בחר **מחק עותקים שלא נקראו של הודעה זו** או **מחק עותקים שלא נקראו והחלף אותם בהודעה חדשה ולאחר** מכן בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="6345f-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="6345f-117">אם אתה שולח הודעה חלופית, חבר את ההודעה ולאחר מכן בחר **שלח**.</span><span class="sxs-lookup"><span data-stu-id="6345f-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="6345f-118">הצלחת או כשל של הודעת אחזור תלויה בהגדרות הנמענים ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="6345f-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="6345f-119">לקבלת מידע נוסף, כולל כיצד לבדוק את האחזור, ראה [אחזור או החלפה של הודעת דואר אלקטרוני ששלחת](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="6345f-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="6345f-120">**_כדי לחפש ולמחוק הודעות דואר אלקטרוני בארגון שלך_**, הדרך הקלה ביותר היא אם אתה מנהל מערכת כללי. אם אינך מנהל מערכת כללי, יש להוסיף את החשבון שלך לקבוצת התפקידים של גילוי אלקטרוני Manager או לתפקיד ניהול חיפוש התאימות.</span><span class="sxs-lookup"><span data-stu-id="6345f-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="6345f-121">כדי למחוק הודעות, יהיה עליך להצטרף לקבוצת התפקידים ' ניהול ארגון ' או לתפקיד הניהול ' חיפוש וניקוי '.</span><span class="sxs-lookup"><span data-stu-id="6345f-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="6345f-122">הרשאות לתפקידים אלה מוקצות [במרכז התאימות של אבטחה &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="6345f-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="6345f-123">[צור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/content-search) כדי לאתר את ההודעה שברצונך למחוק.</span><span class="sxs-lookup"><span data-stu-id="6345f-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="6345f-124">[התחבר אל מרכז התאימות של אבטחה & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6345f-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="6345f-125">אם אתה משתמש ב-Office (אימות רב-גורמי), ראה [התחברות ל-Microsoft 365 Security & מרכז התאימות באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6345f-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
