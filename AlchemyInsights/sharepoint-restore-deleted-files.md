---
title: שחזור קובץ או תיקיה שנמחקו
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707523"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="178c6-102">שחזור קובץ או תיקיה שנמחקו</span><span class="sxs-lookup"><span data-stu-id="178c6-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="178c6-103">SharePoint Online שומר על גיבויים של כל התוכן למשך 14 ימים נוספים מעבר למחיקה בפועל.</span><span class="sxs-lookup"><span data-stu-id="178c6-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="178c6-104">אם לא ניתן לשחזר תוכן באמצעות סל המיחזור או שחזור הקבצים, מנהל מערכת יכול לפנות לתמיכה של Microsoft כדי לבקש שחזור בכל עת בתוך חלון 14 הימים.</span><span class="sxs-lookup"><span data-stu-id="178c6-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="178c6-105">ניתן להשלים שחזורים מגיבויים רק עבור אוספי אתרים או אתרי משנה, לא עבור קבצים, רשימות או ספריות ספציפיות.</span><span class="sxs-lookup"><span data-stu-id="178c6-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="178c6-106">בעת מחיקת פריט או אתר מ-Sharepoint, הוא אינו מוסר מיד.</span><span class="sxs-lookup"><span data-stu-id="178c6-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="178c6-107">פריטים שנמחקו עוברים לסל המיחזור למשך פרק זמן מסוים.</span><span class="sxs-lookup"><span data-stu-id="178c6-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="178c6-108">במהלך זמן זה, באפשרותך לשחזר את הפריטים שמחקת למיקומם המקורי.</span><span class="sxs-lookup"><span data-stu-id="178c6-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="178c6-109">לקבלת פרטים נוספים, בקר בקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="178c6-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="178c6-110">[שחזור פריטים בסל המיחזור של אתר SharePoint](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span><span class="sxs-lookup"><span data-stu-id="178c6-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="178c6-111">שחזור קבצים או תיקיות שנמחקו ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="178c6-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="178c6-112">שחזור אוסף אתרים שנמחק (כולל קבוצה, תקשורת ואתרים אחרים)</span><span class="sxs-lookup"><span data-stu-id="178c6-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="178c6-113">שחזור אתר OneDrive שנמחק</span><span class="sxs-lookup"><span data-stu-id="178c6-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="178c6-114">עבור פעולות סל המיחזור בצובר, מנהלי מערכת עשויים לשקול שימוש ב- [Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="178c6-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="178c6-115">**התכונה 'שחזור קבצים'**</span><span class="sxs-lookup"><span data-stu-id="178c6-115">**Files Restore feature**</span></span>

<span data-ttu-id="178c6-116">אם הרבה מקבצי OneDrive או SharePoint שלך נמחקים, הוחלפו, נפגמו או נגועים על-ידי תוכנות זדוניות, באפשרותך לשחזר את כל הOneDrive או את ספריית SharePoint למועד קודם באמצעות התכונה ' שחזור קבצים '.</span><span class="sxs-lookup"><span data-stu-id="178c6-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="178c6-117">שחזור ספריית OneDrive</span><span class="sxs-lookup"><span data-stu-id="178c6-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="178c6-118">שחזור ספריית מסמכים</span><span class="sxs-lookup"><span data-stu-id="178c6-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

