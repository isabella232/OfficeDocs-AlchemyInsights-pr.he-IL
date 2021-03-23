---
title: פתרון בעיות בכניסה יחידה עבור מכשירים המצורפים של תכלת לספירה
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036170"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="d978d-102">פתרון בעיות בכניסה יחידה עבור מכשירים המצורפים של תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="d978d-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="d978d-103">אם יש לך סביבת Active Directory מקומית (AD) וברצונך להצטרף למחשבים המצורפים לתחום הפרסום שלך ל-תכלת AD, באפשרותך לבצע זאת על-ידי ביצוע הצטרפות היברידית של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="d978d-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="d978d-104">[כיצד לבצע את הפעולות הבאות: תכנון היישום ' הצטרפות ל-Active Directory של Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ' מספק לך את השלבים הקשורים ליישום הצטרפות משולבת של תכלת לספירה בסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="d978d-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="d978d-105">לקבלת מידע נוסף, ראה [קביעת תצורה של מכשירים המצורפים של "תכלת לספירה" עבור Single-Sign מקומית בשימוש ב-Windows שלום לעסקים](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="d978d-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="d978d-106">**בעיות באסימון רענון ראשי (PRT)**</span><span class="sxs-lookup"><span data-stu-id="d978d-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="d978d-107">אסימון רענון ראשי (PRT) הוא פריט מפתח של אימות מודעות מיידיות ב-Windows 10, Windows Server 2016 וגירסאות מתקדמות יותר, iOS ומכשירי Android.</span><span class="sxs-lookup"><span data-stu-id="d978d-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="d978d-108">זהו אסימון אינטרנט של JSON (JWT) שהונפקו במיוחד לברוקרים של Microsoft first, כדי לאפשר כניסה יחידה (SSO) על-פני היישומים המשמשים במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="d978d-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="d978d-109">לקבלת פרטים על האופן שבו PRT מונפק, משמש ומוגן במכשירי Windows 10, ראה [מהו אסימון רענון ראשי?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="d978d-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="d978d-110">**WamDefaultSet: כן ו-AzureADPrt: כן**</span><span class="sxs-lookup"><span data-stu-id="d978d-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="d978d-111">שדות אלה מציינים אם המשתמש הצליח לבצע בהצלחה את הודעת התכלת לספירה בעת כניסה למכשיר.</span><span class="sxs-lookup"><span data-stu-id="d978d-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="d978d-112">אם הערכים הם **לא**, ייתכן שהסיבה לכך היא:</span><span class="sxs-lookup"><span data-stu-id="d978d-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="d978d-113">מפתח אחסון מקולקל ב-TPM המשויך למכשיר בעת רישום (סמן את KeySignTest בעת הפעלת הרשאות מוגברות)</span><span class="sxs-lookup"><span data-stu-id="d978d-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="d978d-114">מזהה כניסה חלופי</span><span class="sxs-lookup"><span data-stu-id="d978d-114">Alternate Login ID</span></span>
- <span data-ttu-id="d978d-115">Proxy של HTTP לא נמצא</span><span class="sxs-lookup"><span data-stu-id="d978d-115">HTTP Proxy not found</span></span>

<span data-ttu-id="d978d-116">כדי לפתור בעיות במכשירים באמצעות הפקודה dsregcmd, ראה [מצב SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="d978d-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
