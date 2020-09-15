---
title: קריאה בלבד עבור הודעת תחזוקה בעת ניסיון להשתמש ב-SharePoint או ב-OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670833"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="8062f-102">קריאה בלבד עבור הודעת תחזוקה בעת ניסיון להשתמש ב-SharePoint או ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="8062f-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="8062f-103">המשתמשים יכולים לקבל הודעת **תחזוקה לקריאה בלבד** בעת ניסיון להשתמש ב-SharePoint או ב-OneDrive עבור אחד מהתרחישים הבאים.</span><span class="sxs-lookup"><span data-stu-id="8062f-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="8062f-104">פעילות תחזוקה מתוכננת או פעילה.</span><span class="sxs-lookup"><span data-stu-id="8062f-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="8062f-105">חפש אותם על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="8062f-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="8062f-106">אירוע בעדיפות גבוהה, שירות פעיל שעשוי להתרחש.</span><span class="sxs-lookup"><span data-stu-id="8062f-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="8062f-107">חפש את כל העלונים/האירועים המפורטים על-ידי ניווט [לתקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8062f-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="8062f-108">תרחיש שחזור מקטין לריפוי אוטומטי שעשוי להתרחש עקב אירועים בלתי צפויים בשרתים שעשויים להימשך פחות מ-30 דקות.</span><span class="sxs-lookup"><span data-stu-id="8062f-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="8062f-109">אין מרכז הודעות או הודעות תקינות של שירות עבור שחזורים משניים אלה, אך אתה אמור לחזור לשגרה בקרוב מאוד.</span><span class="sxs-lookup"><span data-stu-id="8062f-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="8062f-110">במקרים מעטים מאוד שמנו לב שאחד משלושת התרחישים המפורטים לעיל היה הגורם לכך, והשירות שוחזר, אך מטמון הדפדפן של המשתמשים לא נוקה.</span><span class="sxs-lookup"><span data-stu-id="8062f-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="8062f-111">נסה לנקות את מטמון הדפדפן לפני הניווט לאתר.</span><span class="sxs-lookup"><span data-stu-id="8062f-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="8062f-112">בדפדפן Microsoft Edge, בחר **הגדרות**ולאחר מכן בחר באפשרות **פרטיות ואבטחה**.</span><span class="sxs-lookup"><span data-stu-id="8062f-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="8062f-113">תחת **נקה גלישה**, בחר **באפשרות בחר מה לנקות**.</span><span class="sxs-lookup"><span data-stu-id="8062f-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="8062f-114">בחר **קבצי cookie ונתוני אתר אינטרנט שנשמרו**ולאחר מכן בחר **נקה**.</span><span class="sxs-lookup"><span data-stu-id="8062f-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="8062f-115">שלבים אלה עשויים להיות שונים בעת שימוש בדפדפנים אחרים כגון Mozilla Firefox או Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="8062f-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="8062f-116">אפשרות נוספת היא לפתוח את אתר SharePoint או את OneDrive בחלון Inprivate חדש.</span><span class="sxs-lookup"><span data-stu-id="8062f-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>