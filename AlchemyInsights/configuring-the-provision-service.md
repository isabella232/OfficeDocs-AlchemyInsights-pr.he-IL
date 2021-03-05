---
title: קביעת התצורה של שירות הקצאת המשאבים
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482867"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="83826-102">קביעת התצורה של שירות הקצאת המשאבים</span><span class="sxs-lookup"><span data-stu-id="83826-102">Configuring the Provision service</span></span>

<span data-ttu-id="83826-103">לצורך הקצאת משתמשים אוטומטית לעבודה, התכונה ' תכלת לספירה ' דורשת אישורים חוקיים המאפשרים לה להתחבר לממשק ה-API של שירותי אינטרנט של יום העבודה.</span><span class="sxs-lookup"><span data-stu-id="83826-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="83826-104">בהמשך, לחצן ' התקשר לבדיקה ' ביישום יום העבודה לפרסום משתמשים מוודא גם אם הוא מצליח להתחבר לקישור תכלת AD לחיבור סוכן הקצאת משאבים המשויך לתחום הפרסום.</span><span class="sxs-lookup"><span data-stu-id="83826-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="83826-105">אם פורטל התכלת מחזיר שגיאה בעת שמירת האישורים, בצע את השלבים המומלצים שלהלן:</span><span class="sxs-lookup"><span data-stu-id="83826-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="83826-106">ודא שהגדרת את חשבון המשתמש של מערכת שילוב יום העבודה כאמור בסעיף ערכת הלימוד [קביעת התצורה של משתמש מערכת האינטגרציה ביום עבודה](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="83826-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="83826-107">ודא ששירות הקצאת המשאבים של תכלת להתחברות מופעל ופועל בשרת Windows המקומי שלך באמצעות מסוף הניהול של שירותים.</span><span class="sxs-lookup"><span data-stu-id="83826-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="83826-108">באפשרותך גם לבדוק את מצב הסוכן בפורטל ' תכלת ' על-ידי לחיצה על לחצן ' הצג את הסוכנים המקומיים '.</span><span class="sxs-lookup"><span data-stu-id="83826-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="83826-109">ודא שאתה מזין את הערך עבור שדה "יום המשתמש" באמצעות התבנית username@workday-שם הדייר.</span><span class="sxs-lookup"><span data-stu-id="83826-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="83826-110">אם שמות הדיירים של יום העבודה חסרים, האימות של יום העבודה נכשל.</span><span class="sxs-lookup"><span data-stu-id="83826-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="83826-111">אם אתה קובע את התצורה של השילוב עם דייר היישום של יום העבודה, שים לב לשעות הזמן המתוזמנות של דייר יום העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="83826-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="83826-112">יום העבודה מתזמן את הזמן לדיירי היישום שלה בסופי שבוע (בדרך כלל מיום שישי בערב עד שבת בבוקר) וכשלים בקישוריות במהלך חלון זמן זה היא בעיה ידועה הפותרת באופן אוטומטי ברגע שדיירי היישום יחזרו למצב מקוון.</span><span class="sxs-lookup"><span data-stu-id="83826-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="83826-113">במקרים נדירים, ייתכן שתראה שגיאה זו גם אם הסיסמה של משתמש מערכת האינטגרציה השתנתה עקב רענון דייר או אם החשבון נמצא במצב נעול או שפג תוקפו.</span><span class="sxs-lookup"><span data-stu-id="83826-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="83826-114">בדוק את מצב משתמש מערכת האינטגרציה באמצעות מנהל יום העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="83826-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="83826-115">לקבלת פרטים נוספים על קביעת התצורה של יום העבודה לצורך הקצאה אוטומטית, ראה [ערכת לימוד: קביעת התצורה של יום עבודה עבור הקצאת משתמשים אוטומטית](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="83826-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
