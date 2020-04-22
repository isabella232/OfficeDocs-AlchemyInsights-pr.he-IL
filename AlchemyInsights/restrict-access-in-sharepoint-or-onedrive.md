---
title: הגבל גישה ל-SharePoint או OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715885"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="408b9-102">הגבל גישה ל-SharePoint או OneDrive</span><span class="sxs-lookup"><span data-stu-id="408b9-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="408b9-103">ב-SharePoint ו-OneDrive, אתה מגביל את הגישה לפריטים כגון קבצים, תיקיות ורשימות על-ידי הענקת גישה רק לקבוצות או לאנשים שברצונך שתהיה להם גישה.</span><span class="sxs-lookup"><span data-stu-id="408b9-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="408b9-104">כברירת מחדל, הרשאות ב-SharePoint עוברות בירושה מלמעלה בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="408b9-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="408b9-105">לכן, קובץ יורש את הרשאותיו מהתיקיה, שיורשת את ההרשאות שלו מהספריה, היורשת את ההרשאות שלו מהאתר.</span><span class="sxs-lookup"><span data-stu-id="408b9-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="408b9-106">באפשרותך לשתף ברמה גבוהה יותר (כגון על-ידי שיתוף אתר שלם) ולאחר מכן לבטל את הירושה אם אינך מעוניין לשתף את כל הפריטים באתר.</span><span class="sxs-lookup"><span data-stu-id="408b9-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="408b9-107">עם זאת, אנחנו לא ממליצים על זה כי זה הופך את שמירה על ההרשאות מורכבות יותר ומבלבל בעתיד.</span><span class="sxs-lookup"><span data-stu-id="408b9-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="408b9-108">הנה מה שאתה יכול לעשות במקום:</span><span class="sxs-lookup"><span data-stu-id="408b9-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="408b9-109">אם, לדוגמה, ברצונך לשתף את כל התוכן של תיקיה למעט קובץ אחד בו, העבר קובץ זה למיקום חדש שאינו משותף.</span><span class="sxs-lookup"><span data-stu-id="408b9-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="408b9-110">אם יש לך שתי תיקיות משניות בתיקיה וברצונך לשתף תיקיית ממשנה אחת עם קבוצות A ו-B ולאפשר לקבוצה בלבד גישה לתיקיית המשנה השניה, שתף את תיקיית האב בקבוצה A והוסף את קבוצת B לתיקיית משנית הראשונה.</span><span class="sxs-lookup"><span data-stu-id="408b9-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="408b9-111">הפסקת שיתוף של קובץ או תיקיה</span><span class="sxs-lookup"><span data-stu-id="408b9-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

