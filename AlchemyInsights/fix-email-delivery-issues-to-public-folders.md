---
title: לפתור בעיות מסירה של דואר אלקטרוני לתיקיות ציבוריות התומכים בדואר
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401331"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="62c1f-102">לפתור בעיות מסירה של דואר אלקטרוני לתיקיות ציבוריות התומכים בדואר</span><span class="sxs-lookup"><span data-stu-id="62c1f-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="62c1f-103">אם שולחים חיצוניים אין אפשרות לשלוח הודעות אל התיקיות הציבוריות שלך התומכים בדואר, ולקבל שולחים השגיאה: **לא נמצא (550 5.4.1)**, ודא לתחום דואר אלקטרוני עבור התיקיה הציבורית נקבעה כתחום ממסר פנימי של במקום קבוצת מחשבים מוסמכים:</span><span class="sxs-lookup"><span data-stu-id="62c1f-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="62c1f-104">פתח את [מרכז הניהול של Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="62c1f-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="62c1f-105">עבור אל **זרימת דואר** \> **תחומים שהתקבלו**, בחר את התחום המקובל, ולאחר מכן לחץ על **ערוך**.</span><span class="sxs-lookup"><span data-stu-id="62c1f-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="62c1f-106">מאפייני דף זה נפתח, אם לסוג תחום מוגדר **Authoritative**, שנה את הערך ל **ממסר פנימי** ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="62c1f-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="62c1f-107">אם שולחים חיצוניים מקבל שגיאה **שאין לך הרשאה (550 5.7.13)**, הפעל את הפקודה הבאה ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:</span><span class="sxs-lookup"><span data-stu-id="62c1f-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="62c1f-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`לדוגמה, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="62c1f-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="62c1f-109">כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני אל תיקיה ציבורית זו, הוסף את הגישה CreateItems מימין משתמש אנונימי.</span><span class="sxs-lookup"><span data-stu-id="62c1f-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="62c1f-110">לדוגמה, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="62c1f-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
