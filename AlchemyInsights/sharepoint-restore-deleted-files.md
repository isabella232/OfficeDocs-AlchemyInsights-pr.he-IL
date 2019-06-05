---
title: שחזור קובץ שנמחק או תיקיה
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: d5250d75a982c0afc9d3e1b2a43be2ba9c3e8f59
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716508"
---
## <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="38122-102">שחזור קובץ שנמחק או תיקיה</span><span class="sxs-lookup"><span data-stu-id="38122-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="38122-103">SharePoint Online שומר גיבויים של כל התוכן עבור 14 ימים נוספים מעבר המחיקה בפועל.</span><span class="sxs-lookup"><span data-stu-id="38122-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="38122-104">אם אין אפשרות לשחזר את תוכן דרך סל המיחזור או לשחזר קבצים, מנהל מערכת יכול פנה לתמיכה של Microsoft כדי לבקש שחזור עת בתוך חלון 14 יום.</span><span class="sxs-lookup"><span data-stu-id="38122-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="38122-105">ניתן להשלים השחזורים מגיבויים רק עבור אוספי אתרים או אתרי המשנה, לא עבור קבצים ספציפיים, רשימות או ספריות.</span><span class="sxs-lookup"><span data-stu-id="38122-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="38122-106">בעת מחיקת פריט או אתר Sharepoint, אינם מיד מוסרים.</span><span class="sxs-lookup"><span data-stu-id="38122-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="38122-107">פריטים שנמחקו לעבור אל סל המיחזור עבור פרק זמן מסוים.</span><span class="sxs-lookup"><span data-stu-id="38122-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="38122-108">במהלך זמן זה, תוכל לשחזר פריטים שמחקת למיקום המקורי שלהם.</span><span class="sxs-lookup"><span data-stu-id="38122-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="38122-109">לקבלת מידע נוסף, נא בקר הקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="38122-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="38122-110">[שחזור פריטים בסל המיחזור של אתר SharePoint](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="38122-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="38122-111">שחזור קבצים שנמחקו או תיקיות ב- OneDrive</span><span class="sxs-lookup"><span data-stu-id="38122-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/en-us/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="38122-112">שחזור אוסף אתרים שנמחקו (כולל הקבוצה, תקשורת ואתרים אחרים)</span><span class="sxs-lookup"><span data-stu-id="38122-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="38122-113">שחזור אתר OneDrive שנמחקו</span><span class="sxs-lookup"><span data-stu-id="38122-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/en-us/onedrive/restore-deleted-onedrive)

<span data-ttu-id="38122-114">עבור פעולות של סל המיחזור בצובר, מנהלים עשויים שקול [Sharepoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="38122-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

## <a name="files-restore-feature"></a><span data-ttu-id="38122-115">התכונה שחזור קבצים</span><span class="sxs-lookup"><span data-stu-id="38122-115">Files Restore feature</span></span>

<span data-ttu-id="38122-116">אם רבים מהקבצים שלך OneDrive או Sharepoint לקבל נמחקים, מוחלפים, פגום או נגוע על-ידי תוכנות זדוניות, באפשרותך לשחזר את הספריה כולה OneDrive או Sharepoint לזמן קודם באמצעות תכונת שחזור קבצים.</span><span class="sxs-lookup"><span data-stu-id="38122-116">If lots of your OneDrive or Sharepoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="38122-117">שחזור ספריה OneDrive</span><span class="sxs-lookup"><span data-stu-id="38122-117">Restore a OneDrive library</span></span>](https://support.office.com/en-us/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="38122-118">שחזור ספריית מסמכים</span><span class="sxs-lookup"><span data-stu-id="38122-118">Restore a Document library</span></span>](https://support.office.com/en-us/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

