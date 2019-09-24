---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123000"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="1dc8e-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="1dc8e-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="1dc8e-103">עבודה עם PowerShell או סקריפטים בתוך Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="1dc8e-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="1dc8e-104">בקרו בקישורים שלהלן לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="1dc8e-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="1dc8e-105">תחילת התחלת עם מעטפת ניהול מקוונת של SharePoint</span><span class="sxs-lookup"><span data-stu-id="1dc8e-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="1dc8e-106">התחבר ל-SPO PowerShell עם אימות רב-גורמי (משרד הבמה)</span><span class="sxs-lookup"><span data-stu-id="1dc8e-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="1dc8e-107">[תבניות ושיטות עבודה של SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) מכילות ספריה של פקודות PowerShell המאפשרת לך לבצע פעולות ניהול מורכבות כלפי SPO.</span><span class="sxs-lookup"><span data-stu-id="1dc8e-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="1dc8e-108">אם אתה נתקל בבעיות התחברות עם מעטפת ניהול SPO, ודא שעדכנת את הגירסה העדכנית ביותר ונסה [לייבא מחדש את המודול](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) באמצעות *"ייבוא-מודול Microsoft. מקוון. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="1dc8e-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="1dc8e-109">אם אתה מנסה להפעיל סקריפטים של מודל אובייקט בצד הלקוח, יהיה עליך להתקין את ה- [SDK של רכיבי הלקוח המקוונים של Sharepoint](https://www.microsoft.com/download/details.aspx?id=42038) במחשב המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="1dc8e-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="1dc8e-110">אם אתה נתקל בבעיות בהפעלת קבצי script מ-PowerShell, ייתכן שתרצה לשקול להפעיל PowerShell כמנהל ולשנות את [מדיניות הביצוע](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="1dc8e-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>