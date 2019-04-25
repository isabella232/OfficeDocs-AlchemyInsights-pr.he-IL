---
title: שמירת אתר או רשימה כתבנית
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243393"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="cb226-102">שמירת אתר או רשימה כתבנית</span><span class="sxs-lookup"><span data-stu-id="cb226-102">Save site or list as a template</span></span>

<span data-ttu-id="cb226-103">תבניות האתר של SharePoint הם הגדרות והאינטראקטיביות המיועד סביב צורך עסקי מסוים.</span><span class="sxs-lookup"><span data-stu-id="cb226-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="cb226-104">לקבלת מידע נוסף, ראה [שימוש בתבניות כדי ליצור סוגים שונים של אתרי SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="cb226-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="cb226-105">להלן מספר נפוצות בעיות/פתרונות לגבי שמירה אתר או רשימה כתבנית ב- SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="cb226-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="cb226-106">**שמור רשימת אתרים/לחצן תבנית אינו זמין או חסר**.</span><span class="sxs-lookup"><span data-stu-id="cb226-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="cb226-107">מנהלים יהיה עליך לאפשר קובץ Script מותאם אישית כדי להפעיל את תכונות התבנית.</span><span class="sxs-lookup"><span data-stu-id="cb226-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="cb226-108">לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="cb226-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="cb226-109">האתר שמור תבנית הפקודה אינה נתמכת ואת עלולה לגרום לבעיות באתרי משתמשים התשתית פרסום שרת SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cb226-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="cb226-110">**תבנית האתר אין אפשרות ליצור או אינו פועל כראוי**</span><span class="sxs-lookup"><span data-stu-id="cb226-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="cb226-111">התבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) והפעלת לא.</span><span class="sxs-lookup"><span data-stu-id="cb226-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="cb226-112">אם התכונה אינה זמינה להפעיל את אוסף האתרים הנוכחי, לא ניתן להשתמש תבנית האתר כדי ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="cb226-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="cb226-113">בדוק אם כל הרשימות או הספריות לחרוג [סף מגבלה של תצוגת רשימה](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של פריטים 5000 כפי זה יכול לחסום יצירה של תבנית אתר.</span><span class="sxs-lookup"><span data-stu-id="cb226-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="cb226-114">האתר באמצעות משאבים רבים מדי, לכן תבנית האתר חורג ממגבלת 50 מגה-בתים (MB).</span><span class="sxs-lookup"><span data-stu-id="cb226-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="cb226-115">קיימות בעיות הצגת נתונים מתוך רשימה המשתמשת עמודה של בדיקת מידע.</span><span class="sxs-lookup"><span data-stu-id="cb226-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="cb226-116">לקבלת מידע נוסף, ראה [שנוצר על-ידי תבנית הרשימה אינה מציגה נתונים מרשימת בדיקת המידע הנכון ב- SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="cb226-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="cb226-117">לקבלת מידע מפורט יותר אודות בעיות נפוצות ופתרונות נא הפניה, [יצירה ושימוש של תבניות אתר](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="cb226-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

