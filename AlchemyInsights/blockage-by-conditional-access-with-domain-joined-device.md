---
title: אני נחסם על-ידי גישה מותנית עם התקן המצורף לתחום
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036698"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="8375b-102">אני נחסם על-ידי גישה מותנית עם התקן המצורף לתחום</span><span class="sxs-lookup"><span data-stu-id="8375b-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="8375b-103">**כלים מומלצים במיוחד**</span><span class="sxs-lookup"><span data-stu-id="8375b-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="8375b-104">[כלי פותר בעיות של רישום מכשירים](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -הכלי שעוזר לפתור בעיות בבעיות רישום המכשירים הנפוצות ביותר.</span><span class="sxs-lookup"><span data-stu-id="8375b-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="8375b-105">[בדיקת קובץ script של קישוריות לרישום מכשירים](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -קובץ ה-script שעוזר להבטיח שההתקן יוכל לגשת לנקודות קצה של רישום מכשירים תחת חשבון המערכת.</span><span class="sxs-lookup"><span data-stu-id="8375b-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="8375b-106">[קובץ script לניקוי התקן תכלת](https://github.com/mzmaili/AzureADDeviceCleanup) -קובץ ה-script המאפשר לך לחפש ולנהל מכשירים ישנים בסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="8375b-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="8375b-107">להלן כמה סיבות נפוצות לכך שגישה מותנית עשויה להיכשל במכשיר שהצטרף לתחום (תכלת לספירה).</span><span class="sxs-lookup"><span data-stu-id="8375b-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="8375b-108">אין **כPRT מודעות מיידיות במכשיר** -עליך להבטיח שההתקן כולל אסימון רענון ראשי של הודעות מיידיות (PRT).</span><span class="sxs-lookup"><span data-stu-id="8375b-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="8375b-109">לקבלת מידע נוסף אודות PRT, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="8375b-110">כדי לוודא אם יש לך תכלת AD PRT, באפשרותך לבצע `dsregcmd/status` את הפקודה במכשיר ולוודא אם "AzureAdPrt" שווה ל-"כן".</span><span class="sxs-lookup"><span data-stu-id="8375b-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="8375b-111">אם "AzureAdPrt" הוא "NO", בדוק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="8375b-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="8375b-112">**בין אם יש לך סביבה מאוחדת עם AD FS, והיא אינה ניתנת לגישה מרשתות הבית של המשתמשים שלך**: במקרה זה, ודא שנקודות הקצה של usernamemixed "נגישות מהאקסטרא.</span><span class="sxs-lookup"><span data-stu-id="8375b-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="8375b-113">אם הפרסום שלך ב-AD FS ממוקם מאחורי VPN, ודא שהמשתמשים מתחברים אל ה-VPN וכניסה מחדש למכשיר.</span><span class="sxs-lookup"><span data-stu-id="8375b-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="8375b-114">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="8375b-115">**אם ה-TPM של ההתקן פגום, ולכן אין לו אפשרות לאמת את ההתקן**: סמן את התיבה "tpm. msc" כדי לבדוק אם המצב של tpm הוא "מוכן".</span><span class="sxs-lookup"><span data-stu-id="8375b-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="8375b-116">אם לא, `dsregcmd/leave` הפעל ותן להתקן להצטרף מחדש ל-תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="8375b-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="8375b-117">לאחר מכן, נסה שוב.</span><span class="sxs-lookup"><span data-stu-id="8375b-117">Then, try again.</span></span> <span data-ttu-id="8375b-118">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="8375b-119">**אתה משתמש בספק זהויות של צד שלישי, שאינו תומך בפרוטוקול WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="8375b-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="8375b-120">כפי שמתואר במסמכים שלנו, המכשירים ההיברידיים של תכלת לספירה אינם יכולים לפעול במקרה זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="8375b-121">בבקשה עבוד עם ספק הזהויות שלך לתמיכה.</span><span class="sxs-lookup"><span data-stu-id="8375b-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="8375b-122">**המשתמשים משתמשים בדפדפן Chrome ללא חשבונות Windows 10** או **שהסיומת של Office chrome אינם משתמשים באופן אוטומטי ב-PRT במכשירים המצורפים ל-או במכשירים** הקשורים ל-: פעולה זו מובילה לכישלון של כל מדיניות גישה מותנית מבוססת מכשיר, כאשר הודעת השגיאה ' התקן לא רשום ' מוצג.</span><span class="sxs-lookup"><span data-stu-id="8375b-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="8375b-123">כדי להשתמש בדפדפן Chrome כראוי, עליך להתקין את ' חשבונות Windows 10 ' או ' הרחבת Office לדפדפן Chrome של המשתמשים ' דרך SCCM או כוונון.</span><span class="sxs-lookup"><span data-stu-id="8375b-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="8375b-124">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="8375b-125">אם לא ניתן לדחוף את הסיומת מרחוק, הודע למשתמשים להתקין באופן ידני אחת מההרחבות שלעיל כדי לגשת ליישומים מאחורי גישה מותנית מבוססת מכשיר.</span><span class="sxs-lookup"><span data-stu-id="8375b-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="8375b-126">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="8375b-127">**המכשיר היה כהלכה היברידית תכלת כלפי מעלה, אך היא נמחקה בטעות או הפכה ללא זמינה, עקב שינויים בסינכרון ב-תכלת AD Connect או מפורטל תכלת**: אם זה קורה, אובייקט ההתקן אינו מזוהה עוד כמכשיר המצורף לחלוטין, למרות שמצב "AzureAdJoined" ו-"PRT" מופיעים כחוקיים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="8375b-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="8375b-128">כדי לפתור בעיה זו, `dsregcmd/leave` הפעל את המכשירים המושפעים והרשה להם להצטרף מחדש לתכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="8375b-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="8375b-129">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)זה.</span><span class="sxs-lookup"><span data-stu-id="8375b-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="8375b-130">אם המכשירים שלך נמצאים ב-Windows 10, 1809 update, באמצעות VPN/ענן Proxy וראה בעיות במצב "AzureAdPrt" או ביישום כלשהו עם בעיית SSO (outlook אינו מתחבר לתיבת דואר למרות שברשותך PRT), ודא שברשותך תיקון [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) או מצטבר של [עדכון מצטבר](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) כדי למנוע כשלים של PRT במכשירים אלה</span><span class="sxs-lookup"><span data-stu-id="8375b-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















