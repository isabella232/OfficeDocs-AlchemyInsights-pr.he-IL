---
title: הפיכת ניהול גירסאות לזמין ברשימה או בספריה
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.openlocfilehash: d9adb02292132e60af206e2fd7fe3204ff03471f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760517"
---
# <a name="enable-versioning-for-a-sharepoint-list-or-library"></a><span data-ttu-id="c5c44-102">הפיכת ניהול גירסאות לזמין עבור SharePoint רשימה או ספריה</span><span class="sxs-lookup"><span data-stu-id="c5c44-102">Enable versioning for a SharePoint list or library</span></span>


<span data-ttu-id="c5c44-103">כאשר ניהול גירסאות זמין ברשימה או בספריית SharePoint שלך, באפשרותך לאחסן, לעקוב אחר, ולשחזר פריטים ברשימה וקבצים בספריה בכל פעם שהם משתנים.</span><span class="sxs-lookup"><span data-stu-id="c5c44-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="c5c44-104">ניהול גירסאות, יחד עם הגדרות אחרות, כגון ההוצאה, מעניק לך רב פקד התוכן נרשם באתר שלך, באפשרותך לספק ערך אמיתי אם יש לך אי פעם צורך להסתכל או לשחזר גירסה ישנה של פריט או קובץ.</span><span class="sxs-lookup"><span data-stu-id="c5c44-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="c5c44-105">לקבלת מידע נוסף אודות ניהול גירסאות בקר מתחת מאמרים.</span><span class="sxs-lookup"><span data-stu-id="c5c44-105">For more information on versioning please visit the below articles.</span></span>

[<span data-ttu-id="c5c44-106">כיצד פועל ניהול גירסאות ברשימה או בספריה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="c5c44-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

[<span data-ttu-id="c5c44-107">הפעלה וקביעת תצורה של ניהול גירסאות עבור רשימה או ספריה</span><span class="sxs-lookup"><span data-stu-id="c5c44-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f&amp;ui=en-US&amp;rs=en-US&amp;ad=US)

[<span data-ttu-id="c5c44-108">כיצד להציג היסטוריית גירסאות</span><span class="sxs-lookup"><span data-stu-id="c5c44-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

[<span data-ttu-id="c5c44-109">שחזור גירסה קודמת של קובץ ב- OneDrive</span><span class="sxs-lookup"><span data-stu-id="c5c44-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893?ui=en-US&amp;rs=en-US&amp;ad=US)

[<span data-ttu-id="c5c44-110">הצגת גירסאות קודמות של קבצי Office</span><span class="sxs-lookup"><span data-stu-id="c5c44-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

[<span data-ttu-id="c5c44-111">מגבלות של ניהול גירסאות</span><span class="sxs-lookup"><span data-stu-id="c5c44-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

<span data-ttu-id="c5c44-112">הערה: אם אתה לקוח Office 365, ניהול גירסאות כעת מופעלת כברירת מחדל בעת יצירת OneDrive חדש עבור ספריות עסקיים, ישמור באופן אוטומטי את הגירסאות 500 האחרון של מסמך.</span><span class="sxs-lookup"><span data-stu-id="c5c44-112">Note: If you are an Office 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="c5c44-113">פעולה זו תסייע לך למנוע אובדן מסמכים חשובים או נתונים.</span><span class="sxs-lookup"><span data-stu-id="c5c44-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="c5c44-114">אם ברשותך ספריות הקיים שלך OneDrive עבור אתר עסקי או באתר הצוות שלך שאינם כוללים ניהול גירסאות זמין, באפשרותך להפעיל ניהול גירסאות אותם בכל עת.</span><span class="sxs-lookup"><span data-stu-id="c5c44-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


