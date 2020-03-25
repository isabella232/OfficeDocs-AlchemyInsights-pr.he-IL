---
title: לא ניתן להיכנס לצוותים עקב שגיאה autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932044"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="3fd2d-102">לא ניתן להיכנס לצוותים עקב שגיאה autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="3fd2d-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="3fd2d-103">אם האפשרות Seamless SSO זמינה כאימות O365, ייתכן שיהיה צורך להוסיף את כתובת ה- URL "autologon.microsoftazuread-sso.com" לאתרי אינטרא-נט.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="3fd2d-104">אם היא נוספה בעבר לאתרים מהימנים ו-Seamless SSO נמצאת בשימוש, יש להסיר אותה מאתרים מהימנים.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="3fd2d-105">עיין ב- [רשימת פעולות לביצוע של פתרון בעיות ב-Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="3fd2d-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="3fd2d-106">בצע שלבים אלה כדי להוסיף כתובת URL לרשימה 'אתרי אינטרא-נט':</span><span class="sxs-lookup"><span data-stu-id="3fd2d-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="3fd2d-107">פתח את Internet Explorer על-ידי לחיצה על לחצן **התחל**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="3fd2d-108">בתיבת החיפוש, הקלד Internet Explorer ולאחר מכן, ברשימת התוצאות, לחץ על **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="3fd2d-109">לחץ על **כלים** ולאחר מכן לחץ על **אפשרויות אינטרנט**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="3fd2d-110">לחץ על הכרטיסיה **אבטחה**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="3fd2d-111">כעת לחץ על **אתרי אינטרא-נט מקומיים** ולאחר מכן לחץ על הלחצן **אתרים** ולאחר מכן על הלחץ **מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="3fd2d-112">הזן את כתובת ה-URL של אתר האינטרנט ולחץ על **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="3fd2d-113">כשתסיים, לחץ על **סגור**.</span><span class="sxs-lookup"><span data-stu-id="3fd2d-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="3fd2d-114">לקבלת מידע נוסף, ראה [תיעוד עבור פריסת Seamless SSO עבור O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (כולל תהליך מבוסס על מדיניות כדי להוסיף כתובת URL אל אתרי אינטרנט בשלב 3).</span><span class="sxs-lookup"><span data-stu-id="3fd2d-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
