---
title: אפשר כתיבת חוזרת של סיסמה ב- Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560441"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e01fd-102">אפשר כתיבת חוזרת של סיסמה ב- Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e01fd-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e01fd-103">כדי לאפשר כתיבת חוזרת של איפוס סיסמה בשירות עצמי, תחילה אפשר את אפשרות הכתיבה החוזרת ב- Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e01fd-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e01fd-104">מתוך שרת Azure AD Connect, השלם את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e01fd-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e01fd-105">היכנס אל שרת Azure AD Connect שלך והתחל את אשף קביעת התצורה של **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e01fd-106">בדף **הכניסה**, לחץ על **קבע תצורה**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e01fd-107">בדף **משימות נוספות**, בחר **התאם אישית אפשרויות סינכרון** ולאחר מכן לחץ על **הבא**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e01fd-108">בדף **התחבר ל- Azure AD**, הזן אישור מנהל מערכת כללי עבור הדייר שלך, ולאחר מכן לחץ על **הבא**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e01fd-109">בדפי הסינון **ספריות Connect** ו **תחום/OU**, לחץ על **הבא**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e01fd-110">בדף **תכונות אופציונליות**, בחר את התיבה לצד **כתיבת חוזרת של סיסמה** ולחץ על **הבא**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e01fd-111">בדף **מוכן לקבוע תצורה** לחץ על **קבע תצורה** והמתן שהתהליך יסתיים.</span><span class="sxs-lookup"><span data-stu-id="e01fd-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e01fd-112">כשתראה את סיום קביעת התצורה, לחץ על **יציאה**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e01fd-113">כאשר כתיבה חוזרת של סיסמה מופעלת ב- Azure AD Connect, קבע את התצורה של Azure AD SSPR עבור כתיבה חוזרת.</span><span class="sxs-lookup"><span data-stu-id="e01fd-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e01fd-114">כדי לאפשר כתיבה חוזרת של סיסמה ב- SSPR, השלם את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e01fd-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e01fd-115">היכנס אל פורטל Azure באמצעות חשבון מנהל המערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="e01fd-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e01fd-116">חפש אחר **Azure Active Directory** ובחר בו, לחץ על **איפוס סיסמה**, לאחר מכן לחץ על **שילוב מקומי**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e01fd-117">להגדיר את האפשרות עבור **כתוב חזרה סיסמאות לספריה המקומית שלך?** על **כן**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e01fd-118">להגדיר את האפשרות עבור **אפשר למשתמשים לבטל נעילה של חשבונות מבלי לאפס את הסיסמה שלהם?** ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e01fd-119">כשתהיה מוכן, לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e01fd-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e01fd-120">לקבלת מידע נוסף, ראה [אפשר כתיבה לאחור לאיפוס סיסמה בשירות עצמי של Azure Active Directory לסביבה מקומית](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="e01fd-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e01fd-121">כאשר מנהל מערכת מאפס סיסמה של משתמש בפורטל Azure, אם אותו משתמש מפוקח או שה- hash של הסיסמה מסונכרן, הסיסמה נכתבת לאחור למקומי.</span><span class="sxs-lookup"><span data-stu-id="e01fd-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e01fd-122">פונקציונליות זו אינה נתמכת בשלב זה בפורטל הניהול של Office.</span><span class="sxs-lookup"><span data-stu-id="e01fd-122">This functionality is currently not supported in the Office Admin portal.</span></span>