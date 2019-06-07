---
title: צור אתר ב- SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753709"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="27de9-102">צור אתרי SharePoint באמצעות תבניות</span><span class="sxs-lookup"><span data-stu-id="27de9-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="27de9-103">תבניות האתר של SharePoint הם הגדרות והאינטראקטיביות המיועד סביב צורך עסקי מסוים.</span><span class="sxs-lookup"><span data-stu-id="27de9-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="27de9-104">לקבלת מידע נוסף, ראה [שימוש בתבניות כדי ליצור סוגים שונים של אתרי SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="27de9-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="27de9-105">להלן מספר נפוצות בעיות/פתרונות לגבי שמירה אתר או רשימה כתבנית ב- Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="27de9-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="27de9-106">**לחצן תבנית הרשימה site/שמור אינו זמין או חסר**</span><span class="sxs-lookup"><span data-stu-id="27de9-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="27de9-107">מנהלים יהיה עליך לאפשר קובץ Script מותאם אישית כדי להפעיל את תכונות התבנית.</span><span class="sxs-lookup"><span data-stu-id="27de9-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="27de9-108">לקבלת שלבים מפורטים, ראה דוגמאות ושיקולים</span><span class="sxs-lookup"><span data-stu-id="27de9-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="27de9-109">אפשר או מנע בקובץ script מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="27de9-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="27de9-110">האתר שמור תבנית הפקודה אינה נתמכת ואת עלולה לגרום לבעיות באתרי משתמשים התשתית פרסום שרת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27de9-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="27de9-111">תבנית האתר אין אפשרות ליצור או לא יפעל כראוי.</span><span class="sxs-lookup"><span data-stu-id="27de9-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="27de9-112">התבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) והפעלת לא.</span><span class="sxs-lookup"><span data-stu-id="27de9-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="27de9-113">אם התכונה אינה זמינה להפעיל את אוסף האתרים הנוכחי, לא ניתן להשתמש תבנית האתר כדי ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="27de9-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="27de9-114">בדוק אם כל הרשימות או הספריות לחרוג [סף מגבלה של תצוגת רשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של פריטים 5000 כפי זה יכול לחסום יצירה של תבנית אתר.</span><span class="sxs-lookup"><span data-stu-id="27de9-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="27de9-115">האתר באמצעות משאבים רבים מדי, לכן תבנית האתר חורג ממגבלת 50 MB.</span><span class="sxs-lookup"><span data-stu-id="27de9-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="27de9-116">קיימות בעיות הצגת נתונים מתוך רשימה המשתמשת עמודה של בדיקת מידע.</span><span class="sxs-lookup"><span data-stu-id="27de9-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="27de9-117">לקבלת מידע נוסף, ראה [שנוצר על-ידי תבנית הרשימה אינה מציגה נתונים מרשימת בדיקת המידע הנכון ב- SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="27de9-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="27de9-118">לקבלת מידע מפורט יותר אודות בעיות ופתרונות נפוצים, נא בדוק [יצירה ושימוש של תבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="27de9-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



