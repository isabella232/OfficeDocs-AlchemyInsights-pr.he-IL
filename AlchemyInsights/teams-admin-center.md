---
title: מרכז הניהול של Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670365"
---
# <a name="teams-admin-center"></a><span data-ttu-id="fe2dd-102">מרכז הניהול של Teams</span><span class="sxs-lookup"><span data-stu-id="fe2dd-102">Teams Admin Center</span></span>

<span data-ttu-id="fe2dd-103">קבל מידע נוסף על ניהול Teams באמצעות [מרכז הניהול של Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="fe2dd-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="fe2dd-104">אם אינך מצליח לגשת למרכז הניהול של Teams, בדוק את הפריטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="fe2dd-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="fe2dd-105">ודא שאפשרת את [כתובות ה- IP וכתובות ה- URL המתאימות ב- Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) של כל ההתקנים ההיקפיים (חומת אש וכו‘) או בחוקי חומת האש במחשב המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="fe2dd-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="fe2dd-106">ודא שההתחברות שבה אתה משתמש כדי לגשת לפורטל הניהול של Teams מתאימה לשם המשתמש שלך המופיע ב-[פורטל הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="fe2dd-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="fe2dd-107">אם המשתמשים אינם מופיעים במרכז הניהול של Teams, בדוק:</span><span class="sxs-lookup"><span data-stu-id="fe2dd-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="fe2dd-108">האם יצרת משתמשים או רשיונות שהוקצו ב- 24 השעות האחרונות?</span><span class="sxs-lookup"><span data-stu-id="fe2dd-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="fe2dd-109">המתן לפחות 24 שעות לפני פתיחת כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="fe2dd-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="fe2dd-110">ודא שהקצית רשיונות מתאימים?</span><span class="sxs-lookup"><span data-stu-id="fe2dd-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="fe2dd-111">אם יש לך מדריך Active Directory מקומי, ודא [שהערך של msRTCSIP-PrimaryUserAddress או כתובת SIP בשדה ProxyAddresses ב-Active Directory המקומי שלך הוא ייחודי והתבנית תואמת](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) Sip:**Username** של המשתמש [ממרכז הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="fe2dd-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="fe2dd-112">אם בכוונתך לשמור על הפריסה של Skype for Business Server ולהגדיר משתמשים באופן מקומי ומקוון: עקוב אחר **ההגדרה ' הכלאה משולבת עם teams ו-Skype For Business online** ' בלוח הבקרה של Skype For business Server והעברת משתמשים באופן מקוון.</span><span class="sxs-lookup"><span data-stu-id="fe2dd-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
