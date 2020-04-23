---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764262"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="098d0-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="098d0-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="098d0-103">עבודה עם PowerShell או סקריפטים בתוך Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="098d0-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="098d0-104">בקרו בקישורים שלהלן לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="098d0-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="098d0-105">תחילת התחלת עם מעטפת ניהול מקוונת של SharePoint</span><span class="sxs-lookup"><span data-stu-id="098d0-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="098d0-106">התחבר ל-SPO PowerShell עם אימות רב-גורמי (משרד הבמה)</span><span class="sxs-lookup"><span data-stu-id="098d0-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="098d0-107">[תבניות ושיטות עבודה של SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) מכילות ספריה של פקודות PowerShell המאפשרת לך לבצע פעולות ניהול מורכבות כלפי SPO.</span><span class="sxs-lookup"><span data-stu-id="098d0-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="098d0-108">אם אתה נתקל בבעיות התחברות עם מעטפת ניהול SPO, ודא שעדכנת את הגירסה העדכנית ביותר ונסה [לייבא מחדש את המודול](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) באמצעות *"ייבוא-מודול Microsoft. מקוון. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="098d0-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="098d0-109">אם אתה מנסה להפעיל סקריפטים של מודל אובייקט בצד הלקוח, יהיה עליך להתקין את ה- [SDK של רכיבי הלקוח המקוונים של Sharepoint](https://www.microsoft.com/download/details.aspx?id=42038) במחשב המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="098d0-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="098d0-110">אם אתה נתקל בבעיות בהפעלת קבצי script מ-PowerShell, ייתכן שתרצה לשקול להפעיל PowerShell כמנהל ולשנות את [מדיניות הביצוע](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="098d0-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>