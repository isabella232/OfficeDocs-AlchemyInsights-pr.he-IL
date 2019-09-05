---
title: שחזור קובץ או תיקיה שנמחקו
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 1d9937c632212d12883a02860354b6112efd49a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749909"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="d1d2f-102">שחזור קובץ או תיקיה שנמחקו</span><span class="sxs-lookup"><span data-stu-id="d1d2f-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="d1d2f-103">SharePoint Online שומר גיבויים של כל התוכן עבור 14 ימים נוספים מעבר למחיקה בפועל.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="d1d2f-104">אם לא ניתן לשחזר את התוכן באמצעות סל המיחזור או שחזור הקבצים, מנהל מערכת יכול לפנות לתמיכת Microsoft כדי לבקש שחזור בכל עת בתוך החלון של 14 הימים.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="d1d2f-105">ניתן להשלים שחזורים מגיבויים רק עבור אוספי אתרים או אתרי משנה, לא עבור קבצים, רשימות או ספריות מסוימים.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="d1d2f-106">בעת מחיקת פריט או אתר מ-Sharepoint, הוא אינו מוסר באופן מיידי.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="d1d2f-107">פריטים שנמחקו נכנסים לסל המיחזור למשך פרק זמן.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="d1d2f-108">במהלך זמן זה, באפשרותך לשחזר את הפריטים שמחקת למיקומם המקורי.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="d1d2f-109">למידע נוסף, אנא בקרו בקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="d1d2f-110">[שחזר פריטים בסל המיחזור של אתר SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="d1d2f-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="d1d2f-111">שחזור קבצים או תיקיות שנמחקו ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="d1d2f-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="d1d2f-112">שחזור אוסף אתרים שנמחק (כולל קבוצה, תקשורת ואתרים אחרים)</span><span class="sxs-lookup"><span data-stu-id="d1d2f-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="d1d2f-113">שחזור אתר OneDrive שנמחק</span><span class="sxs-lookup"><span data-stu-id="d1d2f-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="d1d2f-114">עבור פעולות של סל מיחזור בצובר, מנהלים עשויים לשקול שימוש ב- [Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="d1d2f-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="d1d2f-115">**התכונה ' שחזור קבצים '**</span><span class="sxs-lookup"><span data-stu-id="d1d2f-115">**Files Restore feature**</span></span>

<span data-ttu-id="d1d2f-116">אם המון שלך OneDrive או קבצי SharePoint למחוק, הוחלף, פגום, או נגוע על ידי תוכנות זדוניות, אתה יכול לשחזר את כל OneDrive או ספריית SharePoint שלך לפעם קודמת באמצעות תכונת שחזור קבצים.</span><span class="sxs-lookup"><span data-stu-id="d1d2f-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="d1d2f-117">שחזור ספריית OneDrive</span><span class="sxs-lookup"><span data-stu-id="d1d2f-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="d1d2f-118">שחזור ספריית מסמכים</span><span class="sxs-lookup"><span data-stu-id="d1d2f-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

