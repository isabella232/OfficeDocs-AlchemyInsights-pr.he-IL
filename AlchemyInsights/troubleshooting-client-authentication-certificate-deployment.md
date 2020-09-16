---
title: פתרון בעיות בפריסה של אישורי אימות לקוח
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658987"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="e02f8-102">פתרון בעיות בפריסה של אישורי אימות לקוח</span><span class="sxs-lookup"><span data-stu-id="e02f8-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="e02f8-103">פרופילי אישורי לקוח של NDES/SCEP ו-PKCS/PFX משמשים בדרך כלל בשילוב עם סוגי פרופילים אחרים כגון Wifi, VPN ודואר אלקטרוני כדי לאפשר למשתמשים לבצע אימות למשאבי חברה.</span><span class="sxs-lookup"><span data-stu-id="e02f8-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="e02f8-104">כאשר סוגי פרופילים אלה מקושרים לפרופיל אישור לקוח, תלויים הפריסה המוצלחת של פרופיל זה.</span><span class="sxs-lookup"><span data-stu-id="e02f8-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="e02f8-105">הגדרת התשתית הראשונית והתצורה המשויכת של פרופיל אישורי לקוח דורשים לעתים קרובות פתרון בעיות.</span><span class="sxs-lookup"><span data-stu-id="e02f8-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="e02f8-106">לקבלת מדריך שלב-אחר-שלב להגדרה מוצלחת של מחבר NDES והדרכה לפתרון בעיות כדי לבודד בעיות בפריסת אישורים, ראה:</span><span class="sxs-lookup"><span data-stu-id="e02f8-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="e02f8-107">קביעת תצורה של תשתית לתמיכה ב-SCEP באמצעות ' כוונון '</span><span class="sxs-lookup"><span data-stu-id="e02f8-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="e02f8-108">מבט כולל לפתרון בעיות של פרופילי אישורים SCEP עם Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="e02f8-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="e02f8-109">השתמש בקבצי ה-script של powershell שאליהם הפניה כדי לסייע באימות התצורה שלך.</span><span class="sxs-lookup"><span data-stu-id="e02f8-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="e02f8-110">לקבלת מידע נוסף, ראה [שלחן סקריפטים של אימות מחבר אישור](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="e02f8-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="e02f8-111">**בעיות נפוצות אחרות**</span><span class="sxs-lookup"><span data-stu-id="e02f8-111">**Other common issues**</span></span>

<span data-ttu-id="e02f8-112">**כאשר אני מנסה להתקין את מחבר אישור ה-intune בשרת מחבר NDES, אני מקבל את ההודעה "אין אפשרות לאמת את הסיסמה בבקשת האישור. ייתכן שכבר נעשה בה שימוש. קבל סיסמה חדשה לשליחה באמצעות בקשה זו.**</span><span class="sxs-lookup"><span data-stu-id="e02f8-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="e02f8-113">הודעה זו משמעותה שעליך להפעיל את התקנת מחבר האישורים כמנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="e02f8-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="e02f8-114">בסביבות מסוימות, השרתים שבהם מופעל אישור ה-intune חייב להשתמש בשרת proxy כדי להתחבר למנגינה, ולכן מחבר האישור חייב להשתמש ב-proxy.</span><span class="sxs-lookup"><span data-stu-id="e02f8-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="e02f8-115">בנסיבות מסוימות, מחבר NDES מתעלם מהגדרות ה-proxy שהוגדרו, וייתכן שיהיה צורך לקבוע את התצורה של הגדרות ה-proxy בעת הפעלת ההקשר הביטחוני של LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="e02f8-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="e02f8-116">הפתרון הוא להפעלת Internet Explorer כמערכת ולקביעת התצורה של proxy ב-IE.</span><span class="sxs-lookup"><span data-stu-id="e02f8-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="e02f8-117">לאחר הפעלה מחדש של שירות מחבר המנגינה, מחבר NDES מתחבר לכיוון המנגינה.</span><span class="sxs-lookup"><span data-stu-id="e02f8-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="e02f8-118">**התקני משתמשים אינם מקבלים עוד אישורי SCEP מ-NDES.**</span><span class="sxs-lookup"><span data-stu-id="e02f8-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="e02f8-119">ייתכן שאישור אימות הלקוח הונפק לשרת NDES, ושצוין במהלך התקנת מחבר NDES, פג תוקפו או חסר.</span><span class="sxs-lookup"><span data-stu-id="e02f8-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="e02f8-120">כדי לפתור:</span><span class="sxs-lookup"><span data-stu-id="e02f8-120">To resolve:</span></span> 
 
1. <span data-ttu-id="e02f8-121">הסר את התקנת מחבר NDES.</span><span class="sxs-lookup"><span data-stu-id="e02f8-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="e02f8-122">השתמש בפרטים אלה כדי לבקש אישור חדש לגבי אימות לקוח או אימות שרת:</span><span class="sxs-lookup"><span data-stu-id="e02f8-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="e02f8-123">שם הנושא: CN = fqdn החיצוני</span><span class="sxs-lookup"><span data-stu-id="e02f8-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="e02f8-124">שם חלופי של נושא (שניהם נדרשים): DNS = fqdn החיצוני, DNS = fqdn הפנימי</span><span class="sxs-lookup"><span data-stu-id="e02f8-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="e02f8-125">התקן מחדש את מחבר NDES באמצעות האישור החדש.</span><span class="sxs-lookup"><span data-stu-id="e02f8-125">Reinstall the NDES connector with the new certificate.</span></span>