---
title: הגדרת ClientAccessServerEnabled ל-True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746415"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="0a703-102">הגדרת ClientAccessServerEnabled ל-True</span><span class="sxs-lookup"><span data-stu-id="0a703-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="0a703-103">אם אינך מצליח לפתוח הודעת דואר אלקטרוני מוצפנת ובמקום זאת אתה רואה קובץ מצורף של **rpmsg** , בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0a703-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="0a703-104">התחבר אל Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0a703-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="0a703-105">כדי להתחבר ל-Exchange Online PowerShell, עליך להיכנס באמצעות חשבון מנהל מערכת כללי או מנהל מערכת של Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a703-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="0a703-106">מ.</span><span class="sxs-lookup"><span data-stu-id="0a703-106">a.</span></span> <span data-ttu-id="0a703-107">פתח את Windows PowerShell ולאחר מכן הפעלת הפקודה הבאה: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="0a703-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="0a703-108">b.</span><span class="sxs-lookup"><span data-stu-id="0a703-108">b.</span></span> <span data-ttu-id="0a703-109">בתיבת הדו **בקשת אישור של Windows PowerShell** , הזן את החשבון שלך בעבודה או בבית הספר והסיסמה שלך, c.</span><span class="sxs-lookup"><span data-stu-id="0a703-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="0a703-110">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="0a703-110">Click **OK**.</span></span> 

2. <span data-ttu-id="0a703-111">הפעלת הפקודה הבאה כדי ליצור הפעלה חדשה:</span><span class="sxs-lookup"><span data-stu-id="0a703-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="0a703-112">מ.</span><span class="sxs-lookup"><span data-stu-id="0a703-112">a.</span></span> <span data-ttu-id="0a703-113">הפעל את הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="0a703-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="0a703-114">הפקודה ' ההפעלה `Get-IRMConfiguration` '.</span><span class="sxs-lookup"><span data-stu-id="0a703-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="0a703-115">סמן את ההגדרה **ClientAccessServerEnabled** .</span><span class="sxs-lookup"><span data-stu-id="0a703-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="0a703-116">מ.</span><span class="sxs-lookup"><span data-stu-id="0a703-116">a.</span></span> <span data-ttu-id="0a703-117">אם ההגדרה **ClientAccessServerEnabled** מוגדרת ל- **False**, הפעלת את ה-cmdlet הבא: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="0a703-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="0a703-118">סגור תמיד את הפעלת powershell באמצעות הפקודה הבאה: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="0a703-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="0a703-119">לקבלת מידע נוסף, ראה [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="0a703-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

