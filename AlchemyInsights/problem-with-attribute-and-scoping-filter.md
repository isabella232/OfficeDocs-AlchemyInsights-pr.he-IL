---
title: בעיה במסנן תכונה ובחירת טווח
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481891"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="328ff-102">בעיה במסנן תכונה ובחירת טווח</span><span class="sxs-lookup"><span data-stu-id="328ff-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="328ff-103">**בעיה בערכי UPN מתנגשים**</span><span class="sxs-lookup"><span data-stu-id="328ff-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="328ff-104">יום העבודה כדי להעביר את יום העבודה של הקצאת משתמשים לפרסום הקצאת משתמשים מציגה הודעת שגיאה **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="328ff-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="328ff-105">הפעולה נכשלה מאחר שערך UPN שהתקבל עבור הוספה/שינוי אינו ייחודי ביערות הרחב.</span><span class="sxs-lookup"><span data-stu-id="328ff-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="328ff-106">פרטי שגיאה: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="328ff-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="328ff-107">הערך **userPrincipalName** שמחבר יום העבודה מנסה להגדיר בעת יצירת חשבון המשתמש המודע שכבר קיים בתחום הפרסום של היעד.</span><span class="sxs-lookup"><span data-stu-id="328ff-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="328ff-108">משמעות הדבר היא ש-(1) המשתמש כבר קיים ובדיקת המזהה התואמת נכשלה עבור המשתמש או (2) שכלל הדור של ה-UPN יצר ערך מתנגש.</span><span class="sxs-lookup"><span data-stu-id="328ff-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="328ff-109">להלן השלבים המוצעים לפתרון:</span><span class="sxs-lookup"><span data-stu-id="328ff-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="328ff-110">אם המשתמש כבר קיים ובדיקת המזהה התואמת נכשלה בקישור של חשבון יום העבודה לחשבון Active Directory, ולאחר מכן בדוק אם התכונה ' מזהה תואם ' (בדרך כלל **employeeID**) ביום העבודה והן בהודעה התאמה מדויקת.</span><span class="sxs-lookup"><span data-stu-id="328ff-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="328ff-111">אם אין להם התאמה, זוהי בעיית נתונים שיש לתקן.</span><span class="sxs-lookup"><span data-stu-id="328ff-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="328ff-112">לדוגמה, אם ה-EmployeeID ביום העבודה הוא 001052 ובמודעה היא 1052, אזי מנגנון הקצאת המשאבים ייכשל לקשר בין שני החשבונות וינסה ליצור משתמש שכבר קיים.</span><span class="sxs-lookup"><span data-stu-id="328ff-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="328ff-113">הפתרון במקרה זה הוא לשנות את ערך **EmployeeID** ב-AD כדי לכלול את האפסים המובילים כדי להפוך אותו ל-001052.</span><span class="sxs-lookup"><span data-stu-id="328ff-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="328ff-114">אם הביטוי היוצר של UPN אינו מייצר ערך ייחודי, שקול להשתמש בפונקציה de-שכפול **SelectUniqueValue** כדי ליצור ערך ייחודי בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="328ff-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="328ff-115">**הקצאת משאבים של ' יום עבודה ' למודעה אינה מציבה את ערך התכונה ' מנהל ' עבור חשבון המשתמש של AD**</span><span class="sxs-lookup"><span data-stu-id="328ff-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="328ff-116">משימת הקצאת המשתמשים של יום העבודה למודעה אינה מגדיר את ערך התכונה **manager** עבור חשבונות משתמשים של AD.</span><span class="sxs-lookup"><span data-stu-id="328ff-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="328ff-117">קיימים שני תרחישים אפשריים כאשר התנהגות זו מופיעה:</span><span class="sxs-lookup"><span data-stu-id="328ff-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="328ff-118">לא ניתן לזהות את המנהל ב-יום עבודה לחשבון משתמש מקביל מתאים מאחר שהמנהל אינו נמצא בטווח.</span><span class="sxs-lookup"><span data-stu-id="328ff-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="328ff-119">בתרחיש של **מספר תחומים של AD** , המנהל ביום עבודה אינו נמצא באותו תחום שבו משתמש המשתמש.</span><span class="sxs-lookup"><span data-stu-id="328ff-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="328ff-120">נסה שלבים אלה כדי לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="328ff-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="328ff-121">אם הגדרת מסנני טווח, בדוק תחילה אם המנהל נמצא בטווח ושהוא עונה על משפט טווח הטווח.</span><span class="sxs-lookup"><span data-stu-id="328ff-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="328ff-122">אם המנהל אינו מספק את מסנן טווח הנתונים, שנה את המסנן כך שהמנהל יהיה גם בטווח של פעולת ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="328ff-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="328ff-123">אם יש לך תחומים מרובים של AD, המחבר מכיל מגבלה ידועה של חוסר יכולת לפתור הפניות בין מנהלי מערכת.</span><span class="sxs-lookup"><span data-stu-id="328ff-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="328ff-124">לקבלת פרטים נוספים על קביעת התצורה של יום העבודה לצורך הקצאה אוטומטית, ראה [ערכת לימוד: קביעת התצורה של יום עבודה עבור הקצאת משתמשים אוטומטית](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="328ff-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













