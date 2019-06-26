---
title: פתרון בעיות של 'פתח באמצעות הסייר' ב- SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: fcaca189741bd68878b1dcfab879e6e0f64e6794
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223641"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b9913-102">פתרון בעיות של 'פתח באמצעות הסייר' ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b9913-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="b9913-103">הפקודה 'פתח באמצעות הסייר' פותחת מופע מקומי של סייר Windows שמציג את מבנה התיקיות בשרת שמארח את אתר SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b9913-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="b9913-104">עם זאת, מומלץ [לסנכרן קבצי SharePoint באמצעות לקוח הסינכרון החדש של OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> אשר מספק את התכונה [קבצים לפי דרישה](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), מכיוון שהוא מספק גישה מקומית לקבצים שלך ומציע את הביצועים הטובים ביותר.</span><span class="sxs-lookup"><span data-stu-id="b9913-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="b9913-105">אם בחרת להשתמש בתצוגת הסייר במקום להשתמש בלקוח הסינכרון החדש, הקפד לפעול בהתאם לשלבים ולשיטות העבודה המומלצות במאמרים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="b9913-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="b9913-106">כיצד ניתן להשתמש בפקודה 'פתח באמצעות הסייר' כדי לפתור בעיות ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b9913-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="b9913-107">העתקה או העברה של קבצי ספריה באמצעות הפקודה 'פתח באמצעות הסייר'</span><span class="sxs-lookup"><span data-stu-id="b9913-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="b9913-108">הערה:  לחצן 'פתח באמצעות הסייר' אינו מופיע בחוויית הספריה החדשה.</span><span class="sxs-lookup"><span data-stu-id="b9913-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b9913-109">לחץ על התפריט הנפתח 'תצוגה' בפינה השמאלית העליונה (שם התפריט הנפתח משתנה בהתאם לתצוגה הנוכחית) ולאחר מכן לחץ על 'הצג בסייר הקבצים'.</span><span class="sxs-lookup"><span data-stu-id="b9913-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="b9913-110">הפקודה 'פתח באמצעות הסייר' ב- SharePoint משתמשת בפקדי ActiveX, ולכן היא נתמכת רק ב- Internet Explorer 10 או ב- Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="b9913-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b9913-111">הפקודה 'פתח באמצעות הסייר' אינה פועלת ב- Windows עם Microsoft Edge,‏ Google Chrome ו- Mozilla Firefox או בפלטפורמת Mac.</span><span class="sxs-lookup"><span data-stu-id="b9913-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b9913-112">בשל כך, ייתכן שהאפשרות 'תצוגת סייר' תופיע באפור.</span><span class="sxs-lookup"><span data-stu-id="b9913-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="b9913-113">[מדוע לחצני רצועת הכלים של SharePoint אינם זמינים או מופיעים באפור](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="b9913-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

