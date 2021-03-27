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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398564"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="146c7-102">מושגי אימות מתקדמים החלים על Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="146c7-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="146c7-103">להלן מושגי האימות המתקדמים החלים על Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="146c7-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="146c7-104">**אימות יזום**</span><span class="sxs-lookup"><span data-stu-id="146c7-104">**Proactive Authentication**</span></span>

<span data-ttu-id="146c7-105">כאשר תפעיל את [המדיניות ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge ינסה לבצע אימות יזום של משתמשים מחוברים באמצעות שירותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="146c7-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="146c7-106">במרווחי זמן קבועים, הוא ישתמש בשירות מקוון כדי לבדוק אם יש מניפסט מעודכן המכיל את התצורה השולטת באימות יזום.</span><span class="sxs-lookup"><span data-stu-id="146c7-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="146c7-107">יתרונות: אימות יזום מאפשר אימות לשירותים עיקריים, כגון דף הכרטיסיה החדשה של Office.</span><span class="sxs-lookup"><span data-stu-id="146c7-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="146c7-108">כמו כן, אם Bing משמש כמנוע החיפוש, אימות יזום משפר את הביצועים של שורת הכתובת ומסייע ליצור תוצאות חיפוש מותאמות אישית לצרכי העסק שלך.</span><span class="sxs-lookup"><span data-stu-id="146c7-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="146c7-109">**Windows Hello CredUI עבור אימות NTLM**</span><span class="sxs-lookup"><span data-stu-id="146c7-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="146c7-110">אם כניסה יחידה (SSO) אינה זמינה כאשר אתר אינטרנט מנסה להיכנס למשתמש באמצעות מנגנון NTLM או משא ומתן, תכונה זו תאפשר למשתמש לשתף את אישורי מערכת ההפעלה עם אתר האינטרנט ולספק את אתגר האימות באמצעות ממשק המשתמש של Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="146c7-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="146c7-111">זרימת כניסה זו תופיע רק ב- Windows 10 ורק עבור משתמשים שלא מקבלים SSO במהלך NTLM או משא ומתן על אתגר.</span><span class="sxs-lookup"><span data-stu-id="146c7-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="146c7-112">**שימוש בסיסמאות שנשמרו כדי להיכנס באופן אוטומטי**</span><span class="sxs-lookup"><span data-stu-id="146c7-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="146c7-113">משתמשים השמירה סיסמאות ב- Microsoft Edge יכולים להפוך כניסה אוטומטית לאתרי אינטרנט שבה הם שמרו אישורים.</span><span class="sxs-lookup"><span data-stu-id="146c7-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="146c7-114">משתמשים יכולים להפעיל או לבטל תכונה זו edge://settings/passwords, ולקבוע את תצורתה במדיניות [מנהל הסיסמאות.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="146c7-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
