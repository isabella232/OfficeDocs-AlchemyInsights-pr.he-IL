---
title: יצירת אתר ב-SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770424"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="a6fea-102">יצירת אתרי SharePoint באמצעות תבניות</span><span class="sxs-lookup"><span data-stu-id="a6fea-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="a6fea-103">היכולת לשמור אתר כתבנית אינה נתמכת עם תקשורת מודרנית או אתרי צוות.</span><span class="sxs-lookup"><span data-stu-id="a6fea-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="a6fea-104">לקבלת מידע נוסף אודות השימוש בתבניות [, ראה שמירה, הורדה וטעינה של אתר SharePoint כתבנית](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="a6fea-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="a6fea-105">להלן כמה בעיות/פתרונות נפוצים לגבי שמירת אתר או רשימה כתבנית ב-Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="a6fea-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="a6fea-106">**לחצן שמירת תבנית של אתר/רשימה אינו זמין או חסר**</span><span class="sxs-lookup"><span data-stu-id="a6fea-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="a6fea-107">מנהלי מערכת יצטרכו לאפשר Script מותאם אישית כדי להפוך את תכונות התבנית לזמינות.</span><span class="sxs-lookup"><span data-stu-id="a6fea-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="a6fea-108">לקבלת שלבים מפורטים, דוגמאות ושיקולים לראות</span><span class="sxs-lookup"><span data-stu-id="a6fea-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="a6fea-109">התרה או מניעה של קובץ script מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="a6fea-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="a6fea-110">הפקודה ' שמור אתר כתבנית ' אינה נתמכת ועלולה לגרום לבעיות באתרים המשתמשים בתשתית הפרסום של SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="a6fea-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="a6fea-111">**אין אפשרות ליצור את תבנית האתר או לא לפעול כראוי**</span><span class="sxs-lookup"><span data-stu-id="a6fea-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="a6fea-112">ייתכן שהתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ולא תפעיל אותה.</span><span class="sxs-lookup"><span data-stu-id="a6fea-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="a6fea-113">אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, אין באפשרותך להשתמש בתבנית האתר כדי ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="a6fea-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="a6fea-114">בדוק אם רשימות או ספריות מסוימות חורגות [ממגבלת הרשימה של מגבלת התצוגה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של 5000 פריטים מאחר שאפשרות זו חוסמת יצירה של תבנית אתר.</span><span class="sxs-lookup"><span data-stu-id="a6fea-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="a6fea-115">ייתכן שהאתר משתמש במשאבים רבים מדי ולכן התבנית של האתר חורגת ממגבלת 50 MB.</span><span class="sxs-lookup"><span data-stu-id="a6fea-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="a6fea-116">קיימות בעיות בהצגת נתונים מרשימה המשתמשת בעמודת בדיקת מידע.</span><span class="sxs-lookup"><span data-stu-id="a6fea-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="a6fea-117">לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="a6fea-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="a6fea-118">לקבלת מידע מפורט יותר אודות בעיות ופתרונות נפוצים, נא בדוק [יצירה ושימוש בתבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="a6fea-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



