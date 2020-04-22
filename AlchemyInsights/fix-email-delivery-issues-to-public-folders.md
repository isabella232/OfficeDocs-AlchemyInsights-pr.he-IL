---
title: תיקון בעיות העברת דואר אלקטרוני לתיקיות ציבוריות התומכות בדואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716353"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="b98d3-102">תיקון בעיות העברת דואר אלקטרוני לתיקיות ציבוריות התומכות בדואר</span><span class="sxs-lookup"><span data-stu-id="b98d3-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="b98d3-103">אם שולחים חיצוניים אינם יכולים לשלוח הודעות לתיקיות הציבוריות המותאמות לדואר שלך, והשולחים מקבלים את השגיאה: **לא נמצא (550 5.4.1)**, ודא שתחום הדואר האלקטרוני עבור התיקיה הציבורית מוגדר כתחום ממסר פנימי במקום תחום סמכותי:</span><span class="sxs-lookup"><span data-stu-id="b98d3-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="b98d3-104">פתח את [מרכז הניהול של Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="b98d3-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="b98d3-105">עבור אל \> **קבוצות מחשבים מקובלות**של **זרימת דואר** , בחר את התחום המקובל ולאחר מכן לחץ על **עריכה**.</span><span class="sxs-lookup"><span data-stu-id="b98d3-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="b98d3-106">בדף המאפיינים שנפתח, אם סוג התחום מוגדר **כסמכותי**, שנה את הערך **לממסר פנימי** ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="b98d3-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="b98d3-107">אם שולחים חיצוניים מקבלים את השגיאה **שאין לך הרשאה (550 5.7.13)**, הפעל את הפקודה הבאה ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:</span><span class="sxs-lookup"><span data-stu-id="b98d3-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="b98d3-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous``Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`. לדוגמא</span><span class="sxs-lookup"><span data-stu-id="b98d3-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="b98d3-109">כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני לתיקיה ציבורית זו, הוסף את הגישה של CreateItems ישירות למשתמש אנונימי.</span><span class="sxs-lookup"><span data-stu-id="b98d3-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="b98d3-110">`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`. לדוגמא</span><span class="sxs-lookup"><span data-stu-id="b98d3-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
