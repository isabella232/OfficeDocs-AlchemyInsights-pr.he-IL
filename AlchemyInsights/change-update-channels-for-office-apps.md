---
title: שינוי ערוצי עדכון עבור יישומי Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439388"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="1837e-102">שינוי ערוצי עדכון עבור יישומי Office</span><span class="sxs-lookup"><span data-stu-id="1837e-102">Change update channels for Office apps</span></span>

<span data-ttu-id="1837e-103">עבור התקנות Office חדשות, השתמש בהגדרות הורדת תוכנה של Office כדי לבחור את ערוץ העדכון הרצוי ולאחר מכן התקן (או התקן מחדש) יישומי Office.</span><span class="sxs-lookup"><span data-stu-id="1837e-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="1837e-104">לקבלת מידע נוסף, ראה [ניהול הגדרות הורדת תוכנה ב-Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="1837e-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="1837e-105">**שים לב** ערוץ העדכון שנבחר באמצעות הגדרות הורדת התוכנה של Office חל על כל המשתמשים המבצעים התקנות חדשות באמצעות הפורטל O365.</span><span class="sxs-lookup"><span data-stu-id="1837e-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="1837e-106">לקבלת מידע נוסף, ראה [הורדת והתקנה או התקנה מחדש של Microsoft 365 או Office 2019 במחשב או ב-Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="1837e-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="1837e-107">עבור התקנות Office קיימות, השתמש בכלי פריסת Office (ODT) כדי לעבור לערוץ עדכונים אחר:</span><span class="sxs-lookup"><span data-stu-id="1837e-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="1837e-108">הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office ( setup.exe ) [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="1837e-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="1837e-109">זהה את שם הערוץ שאליו ברצונך לעבור.</span><span class="sxs-lookup"><span data-stu-id="1837e-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="1837e-110">לקבלת מידע נוסף, ראה [אפשרויות תצורה עבור כלי הפריסה של Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="1837e-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="1837e-111">צור קובץ XML של תצורה המציין את שם הערוץ המתאים, לדוגמה update.xml .</span><span class="sxs-lookup"><span data-stu-id="1837e-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  
    <span data-ttu-id="1837e-112">קצת.</span><span class="sxs-lookup"><span data-stu-id="1837e-112">a.</span></span> <Configuration>  
    <span data-ttu-id="1837e-113">b.</span><span class="sxs-lookup"><span data-stu-id="1837e-113">b.</span></span> <span data-ttu-id="1837e-114"><Updates **ערוץ = "חודשי"** /></span><span class="sxs-lookup"><span data-stu-id="1837e-114"><Updates **Channel="Monthly"** /></span></span>  
    <span data-ttu-id="1837e-115">c.</span><span class="sxs-lookup"><span data-stu-id="1837e-115">c.</span></span> </Configuration>
4. <span data-ttu-id="1837e-116">משורת פקודה עם הרשאות מלאות, עבור למיקום התיקיה שבו הוא setup.exe נמצא והפעל את הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="1837e-116">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="1837e-117">קצת.</span><span class="sxs-lookup"><span data-stu-id="1837e-117">a.</span></span> <span data-ttu-id="1837e-118">setup.exe /קביעת תצורה של update.xml</span><span class="sxs-lookup"><span data-stu-id="1837e-118">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="1837e-119">הפעל יישום של Office (כגון Excel) ולאחר **File**מכן בחר  >  **חשבון**קובץ.</span><span class="sxs-lookup"><span data-stu-id="1837e-119">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="1837e-120">במקטע פרטי מוצר, בחר באפשרות **עדכן אפשרויות**  >  **עדכון כעת**.</span><span class="sxs-lookup"><span data-stu-id="1837e-120">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="1837e-121">לקבלת מידע נוסף, ראה [כיצד להחליף ערוצי עדכון עבור יישומי Office קיימים](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="1837e-121">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="1837e-122">להחלפת ערוצי עדכון עבור קבוצה נבחרת של משתמשים או באמצעות מנהל התצורה (SCCM), הגדר את ההגדרה עדכן ערוץ באמצעות GPO.</span><span class="sxs-lookup"><span data-stu-id="1837e-122">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="1837e-123">לקבלת מידע נוסף, ראה [מבט כולל על ערוצי העדכון של Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="1837e-123">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="1837e-124">לקבלת פרטים, ראה [כיצד לנהל את הערוצים של Office 365 ProPlus עבור מומחי IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) [ולנהל עדכונים ל-Microsoft 365 Apps עם מנהל התצורה של נקודות הקצה של Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="1837e-124">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>