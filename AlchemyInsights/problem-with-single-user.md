---
title: בעיה עם משתמש בודד
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429714"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="6026e-102">בעיה עם משתמש בודד</span><span class="sxs-lookup"><span data-stu-id="6026e-102">Problem with single user</span></span>

- <span data-ttu-id="6026e-103">ייתכן שהמשתמש לא הוקצה מכיוון שהשירות לא הספיק להעריך את המשתמש עדיין.</span><span class="sxs-lookup"><span data-stu-id="6026e-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="6026e-104">סקור את ההדרכה למשך הזמן הדרוש לאספקה ולפס ההתקדמות בדף קביעת התצורה של הקצאת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="6026e-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="6026e-105">אם המצב היציב שצוין במקטע הפרטים הנוספים הוא לפני התאריך שבו המשתמש נוצר/עודכן/נמחק, משמעות הדבר היא שעדיין לא הערכנו את המשתמש.</span><span class="sxs-lookup"><span data-stu-id="6026e-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="6026e-106">בתרחיש זה, הדבר הטוב ביותר לעשות הוא להמתין לסיום שירות הקצאת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="6026e-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="6026e-107">שים לב שהשירות שלנו מודע רק לשינויים במשתמש במערכת המקור (ענן HR).</span><span class="sxs-lookup"><span data-stu-id="6026e-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="6026e-108">חייב להיות שינוי חוקי במערכת המקור עבור תכלת לספירה כדי לזהות את השינוי ולזרום אותו ל-Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6026e-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="6026e-109">שירות הקצאת המשאבים העריך את המשתמש וקבע שאין להקצות אותו:</span><span class="sxs-lookup"><span data-stu-id="6026e-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="6026e-110">אם הגדרת מסנן טווח המבוסס על תכונה, ודא שהמשתמש עומד בקריטריונים שציינת.</span><span class="sxs-lookup"><span data-stu-id="6026e-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="6026e-111">אם המשתמשים כבר קיימים במערכת היעד והמצב של המשתמש בהתאמת המקור והיעד, לא נעשה כל פעולה נוספת.</span><span class="sxs-lookup"><span data-stu-id="6026e-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="6026e-112">שירות הקצאת המשאבים ניסה להקצות את המשתמש והוא נכשל.</span><span class="sxs-lookup"><span data-stu-id="6026e-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="6026e-113">עבור תרחישים אלה, עיין בכרטיסיה פתרון בעיות והמלצות ביומני הקצאת המשאבים:</span><span class="sxs-lookup"><span data-stu-id="6026e-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="6026e-114">ייתכן שתכונה נדרשת במשתמש חסרה במדריך הכתובות המקומי של Active Directory או ב-תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="6026e-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="6026e-115">לדוגמה, כללי הדור של userPrincipalName או sAMAccountName אינם מייצרים את הערך הנכון.</span><span class="sxs-lookup"><span data-stu-id="6026e-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="6026e-116">התכונה התואמת (בדרך כלל employeeId) אינה מתאימה למשתמש ייחודי במדריך הכתובות המקומי של Active Directory או תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="6026e-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="6026e-117">לדוגמה, ישנם שני משתמשים בעלי אותו employeeId ב-AD והשירות מחזיר קוד שגיאה המציין ערכי יעד כפולים עבור אותו ערך מקור.</span><span class="sxs-lookup"><span data-stu-id="6026e-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="6026e-118">כדי לסקור יומני רישום עבור משתמשים וקבוצות בודדים, ראה [סקירת יומני הקצאת המשאבים עבור בעיה במשתמש ספציפי](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="6026e-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
