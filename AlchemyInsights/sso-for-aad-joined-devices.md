---
title: Single-Sign עבור התקנים מצורפים של Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405046"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="f4f04-102">כניסה יחידה עבור מכשירים מצורפים של Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f4f04-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="f4f04-103">אם יש לך סביבת Active Directory (AD) מקומית וברצונך להצטרף למחשבים המצורפים לתחום של AD ל- Azure AD, באפשרותך לבצע זאת על-ידי ביצוע צירוף היברידי של Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4f04-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="f4f04-104">[כיצד לבצע: תכנון יישום ההצטרפות ההיברידי של Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) מספק לך את השלבים הקשורים ליישום צירוף Azure AD היברידי בסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="f4f04-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="f4f04-105">קביעת תצורה של מכשירים מצורפים של Azure AD עבור Single-Sign לשימוש ב- Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="f4f04-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="f4f04-106">**בעיות אסימון רענון ראשי (PRT)** אסימון רענון ראשי (PRT) הוא ממצא מפתח של אימות Azure AD ב- Windows 10 , Windows Server 2016 וגירסאות מתקדמות יותר, מכשירי iOS ו- Android.</span><span class="sxs-lookup"><span data-stu-id="f4f04-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="f4f04-107">זהו אסימון אינטרנט של JSON (JWT) שהונפק במיוחד ל- Microsoft first token brokers כדי להפוך כניסה יחידה (SSO) לזמינה בכל היישומים המשמשים במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="f4f04-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="f4f04-108">[ב מהו אסימון רענון ראשי?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), נספק פרטים אודות אופן ההנפקה, שימוש וההגנה של PRT במכשירי Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f4f04-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="f4f04-109">**WamDefaultSet: YES ו- AzureADPrt: YES** שדות אלה מציינים אם המשתמש מאומת בהצלחה ל- Azure AD בעת הכניסה למכשיר.</span><span class="sxs-lookup"><span data-stu-id="f4f04-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="f4f04-110">אם הערכים הם **NO**, ייתכן שתאריך היעד שלו הוא:</span><span class="sxs-lookup"><span data-stu-id="f4f04-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="f4f04-111">מפתח אחסון גרוע ב- TPM המשויך למכשיר בעת הרישום (בדוק את KeySignTest בעת הפעלת הרשאות מלאות).</span><span class="sxs-lookup"><span data-stu-id="f4f04-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="f4f04-112">מזהה כניסה חלופי</span><span class="sxs-lookup"><span data-stu-id="f4f04-112">Alternate Login ID</span></span>
- <span data-ttu-id="f4f04-113">HTTP Proxy לא נמצא</span><span class="sxs-lookup"><span data-stu-id="f4f04-113">HTTP Proxy not found</span></span>

<span data-ttu-id="f4f04-114">פתרון בעיות במכשירים באמצעות הפקודה dsregcmd - [מצב SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="f4f04-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
