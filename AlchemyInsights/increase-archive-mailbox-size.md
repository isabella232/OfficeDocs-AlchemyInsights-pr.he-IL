---
title: 305 הגדלת גודל תיבת הדואר של הארכיון
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778584"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="05caf-102">הגדלת גודל תיבת הדואר של הארכיון</span><span class="sxs-lookup"><span data-stu-id="05caf-102">Increase the archive mailbox size</span></span>


<span data-ttu-id="05caf-103">אם ברצונך לבצע בדיקות אוטומטיות עבור ההגדרות המוזכרות להלן, בחר את לחצן ' הקודם ' < '-בחלק העליון של דף זה, ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שזקוק לגודל תיבת הדואר של הארכיון שלו.</span><span class="sxs-lookup"><span data-stu-id="05caf-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who needs their archive mailbox size increased.</span></span>

<span data-ttu-id="05caf-104">Microsoft 365 [מגביל](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) את הגודל של תיבות דואר של ארכיון בהתבסס על הרשיון שהוקצה לחשבון המשתמש.</span><span class="sxs-lookup"><span data-stu-id="05caf-104">Microsoft 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="05caf-105">כאשר תיבת הדואר של הארכיון מגיעה ל-90% מהגודל המותר, המשתמש מקבל הודעת דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="05caf-105">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="05caf-106">כאשר תיבת דואר של ארכיון מגיעה למגבלת הגודל שלה, המשתמש אינו יכול להעביר פריטים נוספים לתיבת הדואר של הארכיון.</span><span class="sxs-lookup"><span data-stu-id="05caf-106">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="05caf-107">Microsoft 365 אינו מגדיל את הגודל של תיבת דואר של ארכיון לאחר הגעת למגבלת הגודל.</span><span class="sxs-lookup"><span data-stu-id="05caf-107">Microsoft 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="05caf-108">במקום זאת, המשתמשים יכולים לבצע את הפעולות הבאות כדי לפנות שטח בתיבת הדואר של הארכיון:</span><span class="sxs-lookup"><span data-stu-id="05caf-108">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="05caf-109">יצא את הפריטים לקובץ. pst באמצעות Outlook.</span><span class="sxs-lookup"><span data-stu-id="05caf-109">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="05caf-110">מחיקת פריטים מתיבת הדואר של הארכיון.</span><span class="sxs-lookup"><span data-stu-id="05caf-110">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="05caf-111">Microsoft 365 מספק **אחסון בלתי מוגבל** עבור Office 365 Enterprise E3 ו-E5 רשיונות.</span><span class="sxs-lookup"><span data-stu-id="05caf-111">Microsoft 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="05caf-112">מנהל מערכת חייב להפוך תכונה זו לזמינה לפני שתיבת הדואר של הארכיון תגיע לגודל המרבי שלה.</span><span class="sxs-lookup"><span data-stu-id="05caf-112">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="05caf-113">כאשר אחסון בארכיון ללא הגבלה זמין, ניתן להימשך עד 30 יום לפני הוספת שטח פנוי לתיבת הדואר של הארכיון.</span><span class="sxs-lookup"><span data-stu-id="05caf-113">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="05caf-114">לכן, אנו ממליצים למנהלי מערכת לאמת את השטח הפנוי בתיבת הדואר של הארכיון, אשר מאפשרת למשתמש להמשיך להשתמש בתיבת הדואר של הארכיון בזמן שהיא מתרחבת.</span><span class="sxs-lookup"><span data-stu-id="05caf-114">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="05caf-115">לקבלת מידע נוסף, ראה [מבט כולל על ארכיון בלתי מוגבל ב-microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) [והפעלת אחסון בארכיון בלתי מוגבל ב-microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).</span><span class="sxs-lookup"><span data-stu-id="05caf-115">For more information, see [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and [Enable unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="05caf-116">לקבלת מידע נוסף אודות גישה לתיבת הדואר של הארכיון מ-Outlook, ראה [דרישות Outlook לגישה לפריטים בארכיון מורחב אוטומטית](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span><span class="sxs-lookup"><span data-stu-id="05caf-116">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="05caf-117">כדי לקבוע תצורה של מדיניות שמירה המעבירה באופן אוטומטי פריטים לתיבת הדואר של הארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה עבור תיבות דואר בארגון Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="05caf-117">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Microsoft 365 organization](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="05caf-118">**הערה**: ארכיונים המתרחבים אוטומטית אינם נתמכים עבור תיבות דואר ראשיות ב-Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="05caf-118">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
