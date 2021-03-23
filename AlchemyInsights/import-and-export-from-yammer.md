---
title: ייבוא וייצוא מ-קטרת
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036125"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="c6303-102">ייבוא וייצוא מ-קטרת</span><span class="sxs-lookup"><span data-stu-id="c6303-102">Import and export from Yammer</span></span>

<span data-ttu-id="c6303-103">**ייבוא**</span><span class="sxs-lookup"><span data-stu-id="c6303-103">**Import**</span></span>

<span data-ttu-id="c6303-104">אפשרויות ייבוא משתמשים משתנות בהתאם לשאלה אם רשת קטרת שלך נמצאת [במצב מקורי עבור Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)או לא.</span><span class="sxs-lookup"><span data-stu-id="c6303-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="c6303-105">**מצב שאינו מקורי**: ניתן לייבא משתמשים לקבוצות באמצעות [הוסף מפנקס הכתובות](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (מגבלה למשתמשי 100) בתוך הגדרות קבוצה, או ברשת באמצעות [עדכון בצובר](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) בתוך מנהל הרשת.</span><span class="sxs-lookup"><span data-stu-id="c6303-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="c6303-106">**מצב מקורי**: יש לבצע את החברות בקבוצה ואת פעולות החברות ברשת [מפורטל הניהול של Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [מפורטל תכלת לספירה](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), או באמצעות אפשרות אחרת של כרטיס לספירה.</span><span class="sxs-lookup"><span data-stu-id="c6303-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="c6303-107">לרשתות במצב מקורי אין עוד גישה לעדכון בצובר ולתכונות מדור קודם אחר.</span><span class="sxs-lookup"><span data-stu-id="c6303-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c6303-108">קטרת מעולם לא תמך בייבוא תוכן מתוך מנהל הרשת גם כאשר נעשה שימוש בתכונת ייצוא הנתונים ברשת אחרת.</span><span class="sxs-lookup"><span data-stu-id="c6303-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="c6303-109">ניתן לפרסם מחדש תוכן על-ידי פתרונות שותפים או ממשקי Api של קטרת REST.</span><span class="sxs-lookup"><span data-stu-id="c6303-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="c6303-110">**ייצוא**</span><span class="sxs-lookup"><span data-stu-id="c6303-110">**Export**</span></span>

<span data-ttu-id="c6303-111">[ייצוא נתוני רשת בתוך מנהל הרשת](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) מאפשר ייצוא תוכן מרשתות קטרת, כולל הודעות וקבצים.</span><span class="sxs-lookup"><span data-stu-id="c6303-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="c6303-112">קבצים מצורפים יכולים להיות גדולים מאוד ולגרום לייצוא להשלים זמן משמעותי.</span><span class="sxs-lookup"><span data-stu-id="c6303-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="c6303-113">מומלץ לייצא רשתות פעילות באמצעות ה- [API של ייצוא הנתונים](https://developer.yammer.com/docs/data-export-api) בגושים לפי יום או שבוע.</span><span class="sxs-lookup"><span data-stu-id="c6303-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="c6303-114">התמיכה של Microsoft אינה מספקת קבצי script מותאמים אישית למטרה זו.</span><span class="sxs-lookup"><span data-stu-id="c6303-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="c6303-115">[ייצוא GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) נפרד קיים כדי לייצא תוכן עבור משתמש בודד.</span><span class="sxs-lookup"><span data-stu-id="c6303-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>