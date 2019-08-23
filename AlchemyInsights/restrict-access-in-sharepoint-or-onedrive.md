---
title: הגבל גישה ב- SharePoint או OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551452"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="98444-102">הגבל גישה ב- SharePoint או OneDrive</span><span class="sxs-lookup"><span data-stu-id="98444-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="98444-103">ב- SharePoint ו- OneDrive, להגביל גישה לפריטים כגון קבצים, תיקיות ורשימות על-ידי הענקת גישה רק קבוצות או אנשים שברצונך ש- access.</span><span class="sxs-lookup"><span data-stu-id="98444-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="98444-104">כברירת מחדל, עוברות בירושה הרשאות ב- SharePoint מתוך למעלה גבוהה יותר בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="98444-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="98444-105">כך קובץ יורש את הרשאותיו מהתיקיה, יורש את הרשאותיו מספריית, יורש את הרשאותיו מהאתר.</span><span class="sxs-lookup"><span data-stu-id="98444-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="98444-106">באפשרותך לשתף ברמה גבוהה יותר (כגון על-ידי שיתוף אתר שלם) ולאחר מכן לשבור ירושה אם אינך מעוניין לשתף את כל הפריטים באתר.</span><span class="sxs-lookup"><span data-stu-id="98444-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="98444-107">עם זאת, לא מומלץ זה מאחר שהוא מבצע שמירה על ההרשאות מבלבלות ובלתי מורכבים יותר בעתיד.</span><span class="sxs-lookup"><span data-stu-id="98444-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="98444-108">הנה מה שאתה יכול לעשות במקום זאת:</span><span class="sxs-lookup"><span data-stu-id="98444-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="98444-109">אם, לדוגמה, ברצונך לשתף את התוכן של תיקיה למעט קובץ אחד בתוכה, להעביר קובץ זה אל מיקום חדש אשר אינו משותף.</span><span class="sxs-lookup"><span data-stu-id="98444-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="98444-110">אם יש לך שתי תיקיות משנה בתיקיה, וברצונך לשתף תיקיית משנה אחת עם קבוצות A ו- B ואפשר רק לקבוצה A גישה לתיקיית המשנה השני, שיתוף תיקיית האב עם קבוצת A ולהוסיף מקבוצה B לתיקיית המשנה הראשון.</span><span class="sxs-lookup"><span data-stu-id="98444-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="98444-111">הפסק שיתוף קובץ או תיקיה</span><span class="sxs-lookup"><span data-stu-id="98444-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

