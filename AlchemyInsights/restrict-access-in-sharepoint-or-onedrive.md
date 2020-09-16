---
title: הגבל גישה ב-SharePoint או ב-OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720683"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="1a82f-102">הגבל גישה ב-SharePoint או ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="1a82f-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="1a82f-103">ב-SharePoint וב-OneDrive, עליך להגביל את הגישה לפריטים כגון קבצים, תיקיות ורשימות על-ידי הענקת גישה רק לקבוצות או לאנשים שברצונך לקבל גישה אליהם.</span><span class="sxs-lookup"><span data-stu-id="1a82f-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="1a82f-104">כברירת מחדל, הרשאות ב-SharePoint עוברות בירושה מלמעלה למעלה בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="1a82f-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="1a82f-105">כך שקובץ יירש את ההרשאות שלו מהתיקיה, אשר יורשת את ההרשאות שלו מהספריה, אשר יורשת את ההרשאות שלו מהאתר.</span><span class="sxs-lookup"><span data-stu-id="1a82f-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="1a82f-106">באפשרותך לשתף ברמה גבוהה יותר (כגון על-ידי שיתוף אתר שלם) ולאחר מכן לבטל את הירושה אם אינך מעוניין לשתף את כל הפריטים באתר.</span><span class="sxs-lookup"><span data-stu-id="1a82f-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="1a82f-107">עם זאת, איננו ממליצים על אפשרות זו מכיוון שהיא מאפשרת לשמור על ההרשאות מורכבות יותר ומבלבלות בעתיד.</span><span class="sxs-lookup"><span data-stu-id="1a82f-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="1a82f-108">להלן הפעולות שתוכל לבצע במקום זאת:</span><span class="sxs-lookup"><span data-stu-id="1a82f-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="1a82f-109">לדוגמה, אם ברצונך לשתף את כל התוכן של תיקיה למעט קובץ אחד, העבר את הקובץ למיקום חדש שאינו משותף.</span><span class="sxs-lookup"><span data-stu-id="1a82f-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="1a82f-110">אם יש לך שתי תיקיות משנה בתיקיה, וברצונך לשתף תיקיית משנה אחת עם קבוצות A ו-B ולאפשר לקבץ רק גישה לתיקיית המשנה השניה, לשתף את תיקיית האב עם קיבוץ A והוספת קבוצה ב' לתיקיית המשנה הראשונה.</span><span class="sxs-lookup"><span data-stu-id="1a82f-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="1a82f-111">הפסקת שיתוף קובץ או תיקיה </span><span class="sxs-lookup"><span data-stu-id="1a82f-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

