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
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797549"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="6ece1-102">שחזור קובץ או תיקיה שנמחקו</span><span class="sxs-lookup"><span data-stu-id="6ece1-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="6ece1-103">SharePoint Online שומר על גיבויים של כל התוכן למשך 14 ימים נוספים מעבר למחיקה בפועל.</span><span class="sxs-lookup"><span data-stu-id="6ece1-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="6ece1-104">אם לא ניתן לשחזר תוכן באמצעות סל המיחזור או שחזור הקבצים, מנהל מערכת יכול לפנות לתמיכה של Microsoft כדי לבקש שחזור בכל עת בתוך חלון 14 הימים.</span><span class="sxs-lookup"><span data-stu-id="6ece1-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="6ece1-105">ניתן להשלים שחזורים מגיבויים רק עבור אוספי אתרים או אתרי משנה, לא עבור קבצים, רשימות או ספריות ספציפיות.</span><span class="sxs-lookup"><span data-stu-id="6ece1-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="6ece1-106">בעת מחיקת פריט או אתר מ-Sharepoint, הוא אינו מוסר מיד.</span><span class="sxs-lookup"><span data-stu-id="6ece1-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="6ece1-107">פריטים שנמחקו עוברים לסל המיחזור למשך פרק זמן מסוים.</span><span class="sxs-lookup"><span data-stu-id="6ece1-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="6ece1-108">במהלך זמן זה, באפשרותך לשחזר את הפריטים שמחקת למיקומם המקורי.</span><span class="sxs-lookup"><span data-stu-id="6ece1-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="6ece1-109">לקבלת פרטים נוספים, בקר בקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="6ece1-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="6ece1-110">[שחזור פריטים בסל המיחזור של אתר SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="6ece1-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="6ece1-111">שחזור קבצים או תיקיות שנמחקו ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="6ece1-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="6ece1-112">שחזור אוסף אתרים שנמחק (כולל קבוצה, תקשורת ואתרים אחרים)</span><span class="sxs-lookup"><span data-stu-id="6ece1-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="6ece1-113">שחזור אתר OneDrive שנמחק</span><span class="sxs-lookup"><span data-stu-id="6ece1-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="6ece1-114">עבור פעולות סל המיחזור בצובר, מנהלי מערכת עשויים לשקול שימוש ב- [Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="6ece1-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="6ece1-115">**התכונה 'שחזור קבצים'**</span><span class="sxs-lookup"><span data-stu-id="6ece1-115">**Files Restore feature**</span></span>

<span data-ttu-id="6ece1-116">אם הרבה מקבצי OneDrive או SharePoint שלך נמחקים, הוחלפו, נפגמו או נגועים על-ידי תוכנות זדוניות, באפשרותך לשחזר את כל הOneDrive או את ספריית SharePoint למועד קודם באמצעות התכונה ' שחזור קבצים '.</span><span class="sxs-lookup"><span data-stu-id="6ece1-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="6ece1-117">שחזור ספריית OneDrive</span><span class="sxs-lookup"><span data-stu-id="6ece1-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="6ece1-118">שחזור ספריית מסמכים</span><span class="sxs-lookup"><span data-stu-id="6ece1-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

