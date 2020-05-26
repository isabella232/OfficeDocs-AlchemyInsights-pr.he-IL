---
title: 'סורק AIP: התקנה וקביעת תצורה'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358097"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="d3014-102">סורק AIP: התקנה וקביעת תצורה</span><span class="sxs-lookup"><span data-stu-id="d3014-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="d3014-103">**כדי להתקין את סורק AIP, בצע את ההנחיות המומלצות**:</span><span class="sxs-lookup"><span data-stu-id="d3014-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="d3014-104">אם אתה משדרג ולא מבצע התקנה נקייה, אנא ודא שעקבת אחר ההנחיות [לשדרוג הסורק הגנה מפני מידע תכלת](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ועבור לקוח מאוחד לתיוג, ראה [שדרוג סורק הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="d3014-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="d3014-105">ודא שאתה מציית לכל [הדרישות של חומות האש והגדרות התשתית הרשת](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="d3014-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="d3014-106">ודא [שפריטי המדיניות מוגדרים](https://docs.microsoft.com/azure/information-protection/configure-policy) לתיוג אוטומטי או שתווית ברירת מחדל מוגדרת במדיניות.</span><span class="sxs-lookup"><span data-stu-id="d3014-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="d3014-107">ודא שסוג הקובץ הרלוונטי מוגדר עבור תווית/הגנה כמתואר [בסוגי קבצים הנתמכים על-ידי לקוח ' הגנת מידע תכלת '](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="d3014-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="d3014-108">בנוסף, אם ברצונך לשנות את אופן הפעולה המוגדר כברירת מחדל, פעל לפי ההנחיות הבאות: [שינוי רמת ההגנה המהווה ברירת מחדל של קבצים](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="d3014-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="d3014-109">ודא שלחשבון המשתמש המוגדר להפעלת שירות הסורק יש הרשאות גישה לכל המאגרים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="d3014-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="d3014-110">אם אתה עדיין נתקל בבעיות, אנא יצא את יומני הרישום של הסורק והוסף אותם לכרטיס התמיכה.</span><span class="sxs-lookup"><span data-stu-id="d3014-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="d3014-111">**ייצוא הגנה מידע תכלת הסורק יומנים**</span><span class="sxs-lookup"><span data-stu-id="d3014-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="d3014-112">נווט ל-%Localappנתונים\mvsip בהקשר המשתמש המפעיל את שירות הסורק.</span><span class="sxs-lookup"><span data-stu-id="d3014-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="d3014-113">לסגור את כל התוכן תחת התיקיה MSIP.</span><span class="sxs-lookup"><span data-stu-id="d3014-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="d3014-114">שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת השירות שלך.</span><span class="sxs-lookup"><span data-stu-id="d3014-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="d3014-115">אתה יכול גם להשתמש [ייצוא-AIPLogs-Onbeחצאי של](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="d3014-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="d3014-116">**לקבלת מידע נוסף, ראה**:</span><span class="sxs-lookup"><span data-stu-id="d3014-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="d3014-117">פריסת הסורק הגנת מידע תכלת כדי לסווג ולהגן באופן אוטומטי על קבצים</span><span class="sxs-lookup"><span data-stu-id="d3014-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="d3014-118">ציון ושימוש בפרמטר Token עבור הגדרת אימות</span><span class="sxs-lookup"><span data-stu-id="d3014-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="d3014-119">הפעלת מחזור גילוי והצגת דוחות עבור הסורק</span><span class="sxs-lookup"><span data-stu-id="d3014-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="d3014-120">סקירת התיעוד של הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d3014-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d3014-121">דרישות להגנה מפני מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d3014-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="d3014-122">הורד את לקוח הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="d3014-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
