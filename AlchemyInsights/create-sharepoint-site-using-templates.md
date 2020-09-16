---
title: יצירת אתר ב-SharePoint Online
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
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732226"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="0a1ad-102">יצירת אתרי SharePoint באמצעות תבניות</span><span class="sxs-lookup"><span data-stu-id="0a1ad-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="0a1ad-103">היכולת לשמור אתר כתבנית אינה נתמכת בתקשורת מודרנית או באתרי צוות.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="0a1ad-104">לקבלת מידע נוסף אודות השימוש בתבניות [, ראה שמירה, הורדה והעלאה של אתר SharePoint כתבנית](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="0a1ad-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="0a1ad-105">להלן כמה בעיות נפוצות/פתרונות לגבי שמירת אתר או רשימה כתבנית ב-Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="0a1ad-106">**לחצן ' שמירת אתר/תבנית רשימה ' אינו זמין או חסר**</span><span class="sxs-lookup"><span data-stu-id="0a1ad-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="0a1ad-107">מנהלי מערכת יצטרכו לאפשר סקריפט מותאם אישית כדי להפוך את תכונות התבנית לזמינות.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="0a1ad-108">לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה</span><span class="sxs-lookup"><span data-stu-id="0a1ad-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="0a1ad-109">אפשר או מנע סקריפט מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="0a1ad-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="0a1ad-110">הפקודה ' שמור אתר כתבנית ' אינה נתמכת ועלולה לגרום לבעיות באתרים המשתמשים בתשתית הפרסום של SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="0a1ad-111">**לא ניתן ליצור את תבנית האתר או שאינה פועלת כהלכה**</span><span class="sxs-lookup"><span data-stu-id="0a1ad-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="0a1ad-112">ייתכן שלתבנית חסרה [תכונה](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) והיא לא תופעל.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="0a1ad-113">אם התכונה אינה זמינה להפעלה באוסף האתרים הנוכחי, אין באפשרותך להשתמש בתבנית האתר כדי ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="0a1ad-114">בדוק אם רשימות או ספריות חורגות [ממגבלת המגבלה של תצוגת הרשימה](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) של פריטים של 5000, שכן אפשרות זו חוסמת את היצירה של תבנית אתר.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="0a1ad-115">ייתכן שהאתר משתמש במשאבים רבים מדי ולכן תבנית האתר חורגת ממגבלת 50 MB.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="0a1ad-116">קיימות בעיות בהצגת נתונים מתוך רשימה המשתמשת בעמודת בדיקת מידע.</span><span class="sxs-lookup"><span data-stu-id="0a1ad-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="0a1ad-117">לקבלת מידע נוסף, ראה [רשימה שנוצרה על-ידי תבנית אינה מציגה נתונים מרשימת בדיקת המידע הנכונה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="0a1ad-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="0a1ad-118">לקבלת מידע מפורט יותר על בעיות נפוצות ופתרונות, בדוק את [האפשרות צור ושנה תבניות אתר](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="0a1ad-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



