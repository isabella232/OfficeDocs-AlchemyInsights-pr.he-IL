---
title: שמירת אתר או רשימה כתבנית
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727532"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="8ae31-102">שמירת אתר או רשימה כתבנית</span><span class="sxs-lookup"><span data-stu-id="8ae31-102">Save site or list as a template</span></span>

<span data-ttu-id="8ae31-103">תבניות אתר של SharePoint מיועדות להגדרות מוגדרות מוגדרות מסביב לצרכים עסקיים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="8ae31-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="8ae31-104">לקבלת מידע נוסף, ראה [שימוש בתבניות כדי ליצור סוגים שונים של אתרי SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="8ae31-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="8ae31-105">להלן כמה בעיות נפוצות/פתרונות לגבי שמירת אתר או רשימה כתבנית ב-SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8ae31-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="8ae31-106">**לחצן ' שמור תבנית אתר/רשימה ' אינו זמין או חסר**.</span><span class="sxs-lookup"><span data-stu-id="8ae31-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="8ae31-107">מנהלי מערכת יצטרכו לאפשר סקריפט מותאם אישית כדי להפוך את תכונות התבנית לזמינות.</span><span class="sxs-lookup"><span data-stu-id="8ae31-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="8ae31-108">לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה [התרה או מניעה של סקריפט מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8ae31-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="8ae31-109">הפקודה ' שמור אתר כתבנית ' אינה נתמכת ועלולה לגרום לבעיות באתרים המשתמשים בתשתית הפרסום של SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="8ae31-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="8ae31-110">**לא ניתן ליצור את תבנית האתר או שאינה פועלת כהלכה**</span><span class="sxs-lookup"><span data-stu-id="8ae31-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="8ae31-111">ייתכן שלתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) והיא לא תופעל.</span><span class="sxs-lookup"><span data-stu-id="8ae31-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="8ae31-112">אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, אין באפשרותך להשתמש בתבנית האתר כדי ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="8ae31-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="8ae31-113">בדוק אם רשימות או ספריות חורגות [ממגבלת המגבלה של תצוגת הרשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של פריטים של 5000, שכן אפשרות זו חוסמת את היצירה של תבנית אתר.</span><span class="sxs-lookup"><span data-stu-id="8ae31-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="8ae31-114">ייתכן שהאתר משתמש במשאבים רבים מדי ולכן תבנית האתר חורגת ממגבלת 50 מגה-בניות (MB).</span><span class="sxs-lookup"><span data-stu-id="8ae31-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="8ae31-115">קיימות בעיות בהצגת נתונים מתוך רשימה המשתמשת בעמודת בדיקת מידע.</span><span class="sxs-lookup"><span data-stu-id="8ae31-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="8ae31-116">לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="8ae31-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="8ae31-117">לקבלת מידע מפורט יותר על בעיות נפוצות ופתרונות, פנה לכאן [והשתמש בתבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="8ae31-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

