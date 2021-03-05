---
title: קביעת התצורה של שירות הסינכרון של MIM
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481874"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="13ec5-102">קביעת התצורה של שירות הסינכרון של MIM</span><span class="sxs-lookup"><span data-stu-id="13ec5-102">Configure MIM Sync service</span></span>

<span data-ttu-id="13ec5-103">שירות הסינכרון של Microsoft Identity Manager (MIM) הוא רכיב של MIM.</span><span class="sxs-lookup"><span data-stu-id="13ec5-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="13ec5-104">זהו שירות מקומי מרכזי שמאחסן ומשלב מידע עבור ארגונים בעלי ספריות ומסדי נתונים מקומיים מרובים.</span><span class="sxs-lookup"><span data-stu-id="13ec5-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="13ec5-105">ייתכן שתוכל לפתור את הבעיה שלך ב-MIM Sync אם הבעיה טופלה בעדכון האחרון ב-MIM או שהיא אחת מהבעיות האחרות המוזכרות בסעיף הבא.</span><span class="sxs-lookup"><span data-stu-id="13ec5-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="13ec5-106">**שלבים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="13ec5-106">**Recommended steps**</span></span>

1. <span data-ttu-id="13ec5-107">ודא שאתה משתמש בעדכון האחרון של MIM Sync ובדוק את [הערות מהדורת הסינכרון של MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) כדי לקבוע אם הבעיה נפתרה בעדכון.</span><span class="sxs-lookup"><span data-stu-id="13ec5-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="13ec5-108">אם הבעיה היא באמצעות המחבר הכללי של LDAP, SQL כללי, מחבר לוטוס או מחבר שירותי אינטרנט, ודא שאתה משתמש בעדכון אחרון של [המחברים הכלליים](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="13ec5-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="13ec5-109">אם מתבצעת הפסקת סינכרון של MIM באמצעות שגיאה, עיין בטבלה של [קודי שגיאה של ההפעלה](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) כדי לקבוע את הסיבות האפשריות.</span><span class="sxs-lookup"><span data-stu-id="13ec5-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="13ec5-110">אם ההפעלה מפסיקה עם **סיומת-dll-חריגה** ולאחר מכן לחץ על מילים אלה כדי לפתוח את החלון **מאפיינים של אובייקט מחבר** ולאחר מכן לחץ על **מעקב אחר מחסנית...** כדי לראות מידע נוסף על הסיבה הבסיסית, כפי שמתואר [בהרחבה-dll-חריגה](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="13ec5-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="13ec5-111">אם השגיאה שינוי סיסמה של שירות ההודעות (PCNS) מדווחת על **שגיאה 6025** ביומן האירועים במהלך סינכרון סיסמאות, סמן את המדריך לפתרון בעיות [בדיווח של PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)ב-6025.</span><span class="sxs-lookup"><span data-stu-id="13ec5-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="13ec5-112">אם סינכרון מלא עם סוכן ניהול השירות של FIM מתבצע באיטיות, בדוק את ההגדרה ' **הגדל אוטומטית** ' עבור TempDB, כמתואר [בפתרון בעיות בסינכרון מלא או תלוי](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="13ec5-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="13ec5-113">אם אתה נתקל בשגיאה של ' הופסק-שרת ' עם כישלון ביצירה-שירותים באינטרנט-שירותים באמצעות הסוכן הניהול של שירות FIM, ראה [תמיכה-מידע: כשל-יצירה-דרך-אינטרנט-שירותים](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) לקבלת מבט כולל על גורמים.</span><span class="sxs-lookup"><span data-stu-id="13ec5-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

