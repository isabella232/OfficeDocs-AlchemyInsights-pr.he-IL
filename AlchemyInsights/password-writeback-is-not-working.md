---
title: Writeback סיסמה אינו פועל
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243366"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="f1076-102">Writeback סיסמה אינו פועל</span><span class="sxs-lookup"><span data-stu-id="f1076-102">Password Writeback is not working</span></span>

<span data-ttu-id="f1076-103">**אני נתקל בבעיות בקביעת התצורה של הסיסמה writeback**</span><span class="sxs-lookup"><span data-stu-id="f1076-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="f1076-104">סיסמה writeback היא תכונה משופרת.</span><span class="sxs-lookup"><span data-stu-id="f1076-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="f1076-105">ודא שהבנת את דרישות הרישוי:</span><span class="sxs-lookup"><span data-stu-id="f1076-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="f1076-106">דרוש לך רשיון אחד לפחות שהוקצה בארגון שלך</span><span class="sxs-lookup"><span data-stu-id="f1076-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="f1076-107">**משתמשים בענן בלבד** -כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic</span><span class="sxs-lookup"><span data-stu-id="f1076-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="f1076-108">**משתמשים בענן ו/או מקומיים** -תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)</span><span class="sxs-lookup"><span data-stu-id="f1076-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="f1076-109">לקבלת מידע נוסף על דרישות הרישוי, ראה [דרישות רישוי עבור איפוס סיסמה בשירות עצמי של תכלת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="f1076-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="f1076-110">יש לך לפחות חשבון מנהל אחד וחשבון משתמש אחד לבדיקה עם אחד מהרשיונות המתאימים.</span><span class="sxs-lookup"><span data-stu-id="f1076-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="f1076-111">עליך לחבר את האמולטור של התכלת התחברות לאמולטור של בקר התחום הראשי עבור writeback password לעבודה.</span><span class="sxs-lookup"><span data-stu-id="f1076-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="f1076-112">באפשרותך לקבוע את התצורה של מחבר הודעות מיידיות כדי להשתמש בבקר תחום ראשי על-ידי לחיצה ימנית על **המאפיינים** של מחבר הסינכרון של Active directory ולאחר מכן בחירה באפשרות **קבע מחיצות**</span><span class="sxs-lookup"><span data-stu-id="f1076-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="f1076-113">משם, חפש את המקטע **הגדרות חיבור של בקר התחום** וסמן את התיבה שכותרתה **שימוש בבקרי תחום מועדפים בלבד**.</span><span class="sxs-lookup"><span data-stu-id="f1076-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="f1076-114">אם ה-DC המועדף אינו מהווה אמולטור של PDC, הקישור ' תכלת לספירה ' עדיין מגיע אל ה-PDC עבור writeback סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="f1076-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="f1076-115">איפוס הסיסמה הוגדר וזמין בדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="f1076-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="f1076-116">לקבלת מידע נוסף, ראה [הפיכת משתמשים לאיפוס סיסמאות הפרסום התכולים שלהם](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="f1076-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="f1076-117">ודא שחשבון מנהל המערכת המשמש להפיכת סיסמה Writeback הוא חשבון מנהל מערכת בענן (שנוצר באמצעות ' תכלת לספירה לא מקומית ')</span><span class="sxs-lookup"><span data-stu-id="f1076-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="f1076-118">יש לך פריסה מקומית בודדת או מרובת-יערות הפועלת באמצעות פריסה מקומית של Windows Server 2008 R2, Windows Server 2012 או Windows Server 2012 R2 עם ערכות השירות העדכניות ביותר המותקנות</span><span class="sxs-lookup"><span data-stu-id="f1076-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="f1076-119">הכלי ' חיבור למודע תכלת ' מותקן והכנת את סביבת הפרסום שלך לצורך סינכרון לענן.</span><span class="sxs-lookup"><span data-stu-id="f1076-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="f1076-120">לפני שתנסה לבדוק את הסיסמה writeback, ודא שתחילה עליך להשלים את הייבוא המלא והסינכרון המלא מתוך AD ו-תכלת בחיבור של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="f1076-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="f1076-121">לקבלת מידע נוסף, ראה כיצד לבצע [סינכרון מלא וייבוא מלא בחיבור תכלת לספירה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="f1076-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="f1076-122">**אני נתקל בבעיה בקישוריות של writeback סיסמה**</span><span class="sxs-lookup"><span data-stu-id="f1076-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="f1076-123">הורד והפעל את הגירסה העדכנית ביותר של ' [תכלת לספירה](https://www.microsoft.com/download/details.aspx?id=47594) '</span><span class="sxs-lookup"><span data-stu-id="f1076-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="f1076-124">תצורת חומת אש: כלי החיבור של תכלת לספירה (1.1.443 ומעלה) יזדקק לגישת **HTTPS יוצאת** ל:</span><span class="sxs-lookup"><span data-stu-id="f1076-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="f1076-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f1076-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="f1076-126">servicebus. windows. נטוורקס</span><span class="sxs-lookup"><span data-stu-id="f1076-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="f1076-127">אפשר חיבורים לא פעילים להמשך לפחות 2-3 דקות</span><span class="sxs-lookup"><span data-stu-id="f1076-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="f1076-128">**אני עדיין נתקל בבעיות בwriteback סיסמאות**</span><span class="sxs-lookup"><span data-stu-id="f1076-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="f1076-129">אם אתה עדיין נתקל בקשיים, נסה לבטל ולהפעיל מחדש את שירות writeback password בכלי ' חיבור לספירה של תכלת '</span><span class="sxs-lookup"><span data-stu-id="f1076-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="f1076-130">לקבלת מידע נוסף, ראה כיצד [להפוך ללא זמין ולהפעיל מחדש את הסיסמה writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="f1076-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
