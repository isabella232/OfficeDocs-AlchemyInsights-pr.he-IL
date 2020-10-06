---
title: פתרון בעיות במסירת דואר אלקטרוני לתיקיות ציבוריות המותאמות לדואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366465"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="e8545-102">פתרון בעיות במסירת דואר אלקטרוני לתיקיות ציבוריות המותאמות לדואר</span><span class="sxs-lookup"><span data-stu-id="e8545-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="e8545-103">אם שולחים חיצוניים אינם יכולים לשלוח הודעות לתיקיות ציבוריות המותאמות לדואר שלך, והשולחים מקבלים את השגיאה: **לא ניתן למצוא אותו (550 5.4.1)**, לוודא שתחום הדואר האלקטרוני של התיקיה הציבורית מוגדר כתחום ממסר פנימי במקום תחום סמכותי:</span><span class="sxs-lookup"><span data-stu-id="e8545-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="e8545-104">פתח את [מרכז הניהול של Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="e8545-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="e8545-105">עבור אל **Mail flow** \> **תחומים מקובלים**של זרימת דואר, בחר את התחום המקובל ולאחר מכן לחץ על **ערוך**.</span><span class="sxs-lookup"><span data-stu-id="e8545-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="e8545-106">בעמוד המאפיינים שנפתח, אם סוג התחום מוגדר **כסמכותי**, שנה את הערך **לממסר פנימי** ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e8545-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="e8545-107">אם שולחים חיצוניים מקבלים את השגיאה **שאין לך הרשאה (550 5.7.13)**, השתמש בפקודה הבאה ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:</span><span class="sxs-lookup"><span data-stu-id="e8545-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="e8545-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` לדוגמה, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="e8545-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="e8545-109">כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני לתיקיה ציבורית זו, הוסף את הגישה CreateItems ישירות למשתמש בעילום שם.</span><span class="sxs-lookup"><span data-stu-id="e8545-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="e8545-110">לדוגמה, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="e8545-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
