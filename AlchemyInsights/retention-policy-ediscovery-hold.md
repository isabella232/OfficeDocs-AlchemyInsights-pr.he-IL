---
title: 2609-שמירה או גילוי-החזקה
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994068"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="5ebe2-102">אין אפשרות למחוק פריטים ב-SharePoint Online או OneDrive עבור עסקים</span><span class="sxs-lookup"><span data-stu-id="5ebe2-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="5ebe2-103">ייתכן שאין באפשרותך למחוק פריטים ב-SharePoint Online או OneDrive עבור עסקים מאחר שמדיניות שמירה, תווית שמירה או החזקת eDiscovery מוחלת על SharePoint של אתר OneDrive או על פריט מסוים.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="5ebe2-104">הדבר כולל האפשרות למחוק מסמך, גירסת מסמך, תיקיה, ספריית מסמכים, רשימה, יישום, אתר או אוסף אתרים.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="5ebe2-105">להלן מספר דוגמאות להודעות השגיאה שאתה עשוי לקבל אם אתה מנסה למחוק פריט שנשמר:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="5ebe2-106">"אין אפשרות למחוק אתר זה מאחר שהוא נכלל במדיניות החזקה או השמירה של גילוי eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="5ebe2-107">"אתר זה כולל מדיניות תאימות שנקבעה לחסימת המחיקה"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="5ebe2-108">"מדיניות תאימות חוסמת כעת את מחיקת האתר"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="5ebe2-109">"אין אפשרות למחוק אוסף אתרים זה מאחר שהוא מכיל אתרים הנכללים במדיניות החזקה או השמירה של האתר הediscovery"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="5ebe2-110">"עליך למחוק את כל הפריטים בתיקיה זו לפני שתמחק את התיקיה"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="5ebe2-111">"אין אפשרות למחוק גירסאות של פריט זה מכיוון שהיא נמצאת במצב החזקה או מדיניות שמירה"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="5ebe2-112">"אין אפשרות למחוק את הפריט בעת ההמתנה"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="5ebe2-113">"התווית המוחלת על פריט זה מונעת את עריכתו או מחיקתם"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="5ebe2-114">"אין אפשרות למחוק רשימה בעת בהמתנה או מדיניות שמירה"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="5ebe2-115">"אין אפשרות למחוק את הרשימה אם היא חסומה או אם מוחלת עליה מדיניות שמירה"</span><span class="sxs-lookup"><span data-stu-id="5ebe2-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="5ebe2-116">כדי למחוק פריטים באחד מתרחישים אלה, יש להסיר את מדיניות השמירה, את תווית השמירה או את החזקת eDiscovery (או שאתר צריך להיות מנשלל ממדיניות שמירה).</span><span class="sxs-lookup"><span data-stu-id="5ebe2-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="5ebe2-117">עליך להשבית או לא לכלול חסימה בהתאמה שגורמת לבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="5ebe2-118">לאחר הסרת מדיניות שמירה או החזקה, ייתכן שהשינוי ישפיע עד 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="5ebe2-119">לקבלת מידע אודות התכונות השונות של שמירה והחזקה שניתן להחיל על אתרי SharePoint וחשבונות OneDrive, ראה אחד מהנושאים הבאים.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="5ebe2-120">מבט כולל על מדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="5ebe2-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="5ebe2-121">מבט כולל על תוויות שמירה</span><span class="sxs-lookup"><span data-stu-id="5ebe2-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="5ebe2-122">ניהול חסימות ב-eDiscovery מתקדם</span><span class="sxs-lookup"><span data-stu-id="5ebe2-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="5ebe2-123">גילוי eDiscovery מחזיק</span><span class="sxs-lookup"><span data-stu-id="5ebe2-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="5ebe2-124">מדיניות הסגר והמחיקה של אתר מדור קודם</span><span class="sxs-lookup"><span data-stu-id="5ebe2-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
