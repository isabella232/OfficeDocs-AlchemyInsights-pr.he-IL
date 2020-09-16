---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770840"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="48ff0-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="48ff0-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="48ff0-103">עבודה עם PowerShell או קבצי Script בתוך Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="48ff0-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="48ff0-104">בקר בקישורים הבאים לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="48ff0-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="48ff0-105">תחילת העבודה עם מעטפת ניהול של SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="48ff0-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="48ff0-106">התחברות ל-SPO PowerShell באמצעות אימות גורמי</span><span class="sxs-lookup"><span data-stu-id="48ff0-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="48ff0-107">[תבניות ותרגולים של SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) מכילות ספריה של פקודות PowerShell המאפשרת לך לבצע פעולות ניהול מורכבות כלפי SPO.</span><span class="sxs-lookup"><span data-stu-id="48ff0-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="48ff0-108">אם אתה נתקל בבעיות בהתחברות עם מעטפת הניהול של SPO, ודא שעדכנת את הגירסה העדכנית ביותר ונסה [לייבא מחדש את המודול](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) באמצעות *"import-module" Microsoft. Online. SharePoint. PowerShell ".*</span><span class="sxs-lookup"><span data-stu-id="48ff0-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="48ff0-109">אם אתה מנסה לנהל קבצי script של מודל אובייקטים בצד הלקוח, יהיה עליך להתקין את ה- [SDK של רכיבי הלקוח של Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) במחשב המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="48ff0-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="48ff0-110">אם אתה נתקל בבעיות בהפעלת קבצי script מ-PowerShell, ייתכן שתרצה לשקול להפעיל את PowerShell כמנהל מערכת ולשנות את [מדיניות הביצוע](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="48ff0-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>