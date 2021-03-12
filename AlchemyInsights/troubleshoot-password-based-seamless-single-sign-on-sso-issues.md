---
title: פתרון בעיות של כניסה יחידה (SSO) חלקה מבוססת סיסמה
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714769"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="d8a52-102">פתרון בעיות של כניסה יחידה (SSO) חלקה מבוססת סיסמה</span><span class="sxs-lookup"><span data-stu-id="d8a52-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="d8a52-103">כדי ללמוד את היסודות של SSO מבוסס סיסמה, ראה [אימות מבוסס סיסמה עם תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="d8a52-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="d8a52-104">**קביעת תצורה של SSO מבוסס סיסמה**</span><span class="sxs-lookup"><span data-stu-id="d8a52-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="d8a52-105">[קביעת התצורה של כניסה יחידה מבוססת סיסמה-מאמר](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) זה מתקבלת לפרטים נוספים אודות האפשרות SSO מבוססת סיסמה.</span><span class="sxs-lookup"><span data-stu-id="d8a52-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="d8a52-106">אם היישום שאתה מוסיף דורש תצורה מותאמת אישית ועליך להשתמש ב-SSO מבוסס סיסמה, מאמר זה מיועד לך.</span><span class="sxs-lookup"><span data-stu-id="d8a52-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="d8a52-107">[קביעת התצורה של כניסה יחידה מבוססת סיסמה עבור יישומים ב-פרם](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -Proxy של יישום תומך בכמה מצבי כניסה יחידה.</span><span class="sxs-lookup"><span data-stu-id="d8a52-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="d8a52-108">כניסה מבוססת סיסמה מיועדת ליישומים המשתמשים בשילוב של שם משתמש/סיסמה לצורך אימות.</span><span class="sxs-lookup"><span data-stu-id="d8a52-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="d8a52-109">בעת קביעת התצורה של כניסה מבוססת סיסמה עבור היישום, המשתמשים שלך צריכים להיכנס ליישום המקומי פעם אחת.</span><span class="sxs-lookup"><span data-stu-id="d8a52-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="d8a52-110">לאחר מכן, תכלת Active Directory מאחסן את מידע הכניסה ומספק אותו באופן אוטומטי ליישום כאשר המשתמשים שלך ניגשים אליו מרחוק.</span><span class="sxs-lookup"><span data-stu-id="d8a52-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="d8a52-111">כבר היית אמור לפרסם ולבדוק את האפליקציה באמצעות Proxy של יישומים.</span><span class="sxs-lookup"><span data-stu-id="d8a52-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="d8a52-112">אם לא, בצע את השלבים המפורטים [ביישומי פרסום באמצעות האפליקציה ' שימוש ב-תכלת לספירה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) ' ולאחר מכן המשך בקביעת התצורה של SSO מבוסס-סיסמה עבור אפליקציות של ה-פרם</span><span class="sxs-lookup"><span data-stu-id="d8a52-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="d8a52-113">כדי לפתור בעיות ב-SSO מבוסס סיסמה, ראה [פתרון בעיות בכניסה יחידה מבוססת סיסמה בתכלת לספירה](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="d8a52-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
