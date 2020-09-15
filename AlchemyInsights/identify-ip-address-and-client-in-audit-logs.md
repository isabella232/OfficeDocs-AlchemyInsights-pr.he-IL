---
title: זיהוי כתובת IP ולקוח ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668311"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ea449-102">זיהוי כתובת IP ולקוח ביומני ביקורת</span><span class="sxs-lookup"><span data-stu-id="ea449-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ea449-103">כתובת ה-IP התואמת לפעילות על-ידי משתמש או מנהל של Microsoft 365 מוצגת ביומני הביקורת.</span><span class="sxs-lookup"><span data-stu-id="ea449-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ea449-104">פרטי הלקוח נרשמים גם הם.</span><span class="sxs-lookup"><span data-stu-id="ea449-104">The client information is also logged.</span></span> <span data-ttu-id="ea449-105">להלן השלבים לזיהוי מידע כזה</span><span class="sxs-lookup"><span data-stu-id="ea449-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ea449-106">היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ea449-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ea449-107">עבור אל דף **Search**  >  **החיפוש ביומן ביקורת** חיפוש.</span><span class="sxs-lookup"><span data-stu-id="ea449-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ea449-108">אם אתה מעוניין בפעילות ספציפית, בחר אותה מהרשימה **פעילויות** .</span><span class="sxs-lookup"><span data-stu-id="ea449-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ea449-109">אם לא, כל הפעילויות יוחזרו עבור המשתמש שנבחר (הגדרת ברירת המחדל).</span><span class="sxs-lookup"><span data-stu-id="ea449-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ea449-110">**הערה**: ייתכן שפעילויות מסוימות לא יהיו זמינות בתפריט ' **פעילויות** '; עם זאת, פריטי ביקורת אלה יוחזרו אם האפשרות ' הגדרת **תוצאות עבור כל הפעילויות** ' נבחרה (הגדרת ברירת המחדל).</span><span class="sxs-lookup"><span data-stu-id="ea449-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ea449-111">ציין את שם המשתמש בשדה **משתמשים** , בחר את טווח התאריכים המתאים עבור הפעילות ולאחר מכן לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="ea449-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ea449-112">בתוצאות, באפשרותך לראות את כתובת ה-IP של פעילות זו בחלונית התוצאות.</span><span class="sxs-lookup"><span data-stu-id="ea449-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ea449-113">בחר את רשומת הביקורת כדי לראות מידע מפורט **בפרטים** נשלף של (לדוגמה, לקוח, משתמש שביצע פעולה וכן הלאה).</span><span class="sxs-lookup"><span data-stu-id="ea449-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ea449-114">לקבלת מידע נוסף, ראה [איתור כתובת ה-IP של המחשב המשמש לגישה לחשבון שנחשף](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="ea449-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
