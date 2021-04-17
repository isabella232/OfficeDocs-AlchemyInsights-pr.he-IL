---
title: מרכז הניהול של Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826380"
---
# <a name="teams-admin-center"></a><span data-ttu-id="5c419-102">מרכז הניהול של Teams</span><span class="sxs-lookup"><span data-stu-id="5c419-102">Teams Admin Center</span></span>

<span data-ttu-id="5c419-103">קבל מידע נוסף על ניהול Teams באמצעות [מרכז הניהול של Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="5c419-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="5c419-104">אם אינך מצליח לגשת למרכז הניהול של Teams, בדוק את הפריטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5c419-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="5c419-105">ודא שאפשרת את [כתובות ה- IP וכתובות ה- URL המתאימות ב- Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) של כל ההתקנים ההיקפיים (חומת אש וכו‘) או בחוקי חומת האש במחשב המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="5c419-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="5c419-106">ודא שההתחברות שבה אתה משתמש כדי לגשת לפורטל הניהול של Teams מתאימה לשם המשתמש שלך המופיע ב-[פורטל הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="5c419-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="5c419-107">אם המשתמשים אינם מופיעים במרכז הניהול של Teams, בדוק:</span><span class="sxs-lookup"><span data-stu-id="5c419-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="5c419-108">האם יצרת משתמשים או רשיונות שהוקצו ב- 24 השעות האחרונות?</span><span class="sxs-lookup"><span data-stu-id="5c419-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="5c419-109">המתן לפחות 24 שעות לפני פתיחת כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="5c419-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="5c419-110">ודא שהקצית רשיונות מתאימים?</span><span class="sxs-lookup"><span data-stu-id="5c419-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="5c419-111">אם יש לך Active Directory מקומי, ודא שהערך [של msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) או כתובת SIP בשדה ProxyAddresses ב- Active Directory המקומי שלך הוא ייחודי והתבנית תואמת ללגימה:**שם** המשתמש של המשתמש ממרכז הניהול של [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="5c419-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="5c419-112">אם בכוונתך לשמור פריסה של Skype for Business Server ולהגדיר משתמשים ביתיים באופן מקומי ומקוון: פעל בהתאם ל"הגדרת היברידיות עם **Teams ו- Skype for Business Online"** בלוח הבקרה של Skype for Business Server והעביר משתמשים למצב מקוון.</span><span class="sxs-lookup"><span data-stu-id="5c419-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
