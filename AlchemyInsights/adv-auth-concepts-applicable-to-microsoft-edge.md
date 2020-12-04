---
title: מושגי אימות מתקדמים החלים על Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573397"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="09021-102">מושגי אימות מתקדמים החלים על Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="09021-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="09021-103">להלן מושגי אימות מתקדמים החלים על Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="09021-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="09021-104">**אימות פרואקטיבי**</span><span class="sxs-lookup"><span data-stu-id="09021-104">**Proactive Authentication**</span></span>

<span data-ttu-id="09021-105">בעת הפיכת מדיניות [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) לזמינה, Microsoft Edge מנסה לאמת משתמשים בעלי חתימה באופן פרואקטיבי באמצעות microsoft services.</span><span class="sxs-lookup"><span data-stu-id="09021-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="09021-106">במרווחי זמן קבועים, הוא ישתמש בשירות מקוון כדי לחפש מניפסט מעודכן המכיל את התצורה השולטת באימות פרואקטיבי.</span><span class="sxs-lookup"><span data-stu-id="09021-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="09021-107">תועלת: אימות פרואקטיבי מאפשר אימות לשירותי מפתח, כגון דף הכרטיסיה החדשה של Office.</span><span class="sxs-lookup"><span data-stu-id="09021-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="09021-108">כמו כן, אם Bing משמש כמנגנון החיפוש, האימות הפרואקטיבי משפר את הביצועים של שורת הכתובת ועוזר ליצור תוצאות חיפוש המותאמות אישית לצרכי העסק שלך.</span><span class="sxs-lookup"><span data-stu-id="09021-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="09021-109">**Windows שלום CredUI עבור אימות NTLM**</span><span class="sxs-lookup"><span data-stu-id="09021-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="09021-110">אם כניסה יחידה (SSO) אינה זמינה כאשר אתר אינטרנט מנסה להיכנס למשתמש באמצעות מנגנון NTLM או ניהול משא ומתן, תכונה זו מאפשרת למשתמש לשתף את אישורי מערכת ההפעלה עם אתר האינטרנט ולספק את אתגר האימות באמצעות ממשק המשתמש של Windows שלום.</span><span class="sxs-lookup"><span data-stu-id="09021-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="09021-111">זרימת הכניסה מופיעה רק ב-Windows 10 ורק עבור משתמשים שאינם מקבלים את SSO במהלך האתגר של NTLM או ניהול משא ומתן.</span><span class="sxs-lookup"><span data-stu-id="09021-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="09021-112">**שימוש בסיסמאות שמורות כדי להיכנס באופן אוטומטי**</span><span class="sxs-lookup"><span data-stu-id="09021-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="09021-113">משתמשים ששומרים סיסמאות ב-Microsoft Edge יכולים לאפשר כניסה אוטומטית לאתרי אינטרנט שבהם הם שמרו אישורים.</span><span class="sxs-lookup"><span data-stu-id="09021-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="09021-114">המשתמשים יכולים להפעיל או לבטל תכונה זו ב-edge://settings/passwords, ובאפשרותך לקבוע את תצורתה במדיניות [מנהל הסיסמאות](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="09021-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
