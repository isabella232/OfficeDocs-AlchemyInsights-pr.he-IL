---
title: 'סורק AIP: התקנה וקביעת תצורה'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821664"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="31263-102">סורק AIP: התקנה וקביעת תצורה</span><span class="sxs-lookup"><span data-stu-id="31263-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="31263-103">**כדי להתקין את סורק AIP, בצע את ההנחיות המומלצות**:</span><span class="sxs-lookup"><span data-stu-id="31263-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="31263-104">אם אתה משדרג ולא מבצע התקנה נקייה, ודא שעקבת אחר הקווים המנחים לשדרוג סורק [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) וללקוח תיוג מאוחד, ראה שדרוג [הסורק Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="31263-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="31263-105">ודא שאתה מציית לכל דרישות [הגדרות חומת האש ותשתית הרשת.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="31263-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="31263-106">ודא שמדיניות [זו מוגדרת לתיוג](https://docs.microsoft.com/azure/information-protection/configure-policy) אוטומטי או שיש לה תווית ברירת מחדל במדיניות.</span><span class="sxs-lookup"><span data-stu-id="31263-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="31263-107">ודא שסוג הקובץ הרלוונטי מוגדר עבור תווית/הגנה כמתואר בסוגי קבצים הנתמכים [על-ידי לקוח Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="31263-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="31263-108">בנוסף, אם ברצונך לשנות את אופן הפעולה המוגדר כברירת מחדל, בצע את ההנחיות הבאות: [שינוי רמת ההגנה המוגדרת כברירת מחדל של קבצים](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="31263-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="31263-109">ודא שחשבון המשתמש שהוגדר להפעיל את שירות הסורק כולל הרשאות לגשת לכל מאגרי מאגרים שהוגדרו.</span><span class="sxs-lookup"><span data-stu-id="31263-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="31263-110">אם אתה עדיין נתקל בבעיות, ייצא את יומני הסורק והוסף אותם לכרטיס התמיכה שלך.</span><span class="sxs-lookup"><span data-stu-id="31263-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="31263-111">**ייצוא יומנים של סורק הגנה על מידע של Azure**</span><span class="sxs-lookup"><span data-stu-id="31263-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="31263-112">נווט אל %localappdata%\Microsoft\MSIP תחת הקשר המשתמש שבו פועל שירות הסורק.</span><span class="sxs-lookup"><span data-stu-id="31263-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="31263-113">דחוס את כל התוכן תחת התיקיה MSIP.</span><span class="sxs-lookup"><span data-stu-id="31263-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="31263-114">שמור את יומני הרישום במיקום שלך וצרף אותם לבקשת השירות שלך.</span><span class="sxs-lookup"><span data-stu-id="31263-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="31263-115">באפשרותך גם להשתמש [בייצוא-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="31263-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="31263-116">**לקבלת מידע נוסף, ראה**:</span><span class="sxs-lookup"><span data-stu-id="31263-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="31263-117">פריסת סורק Azure Information Protection כדי לסווג ולהגן באופן אוטומטי על קבצים</span><span class="sxs-lookup"><span data-stu-id="31263-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="31263-118">ציין את הפרמטר Token והשתמש בו עבור Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="31263-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="31263-119">הפעלת מחזור גילוי ו הצגת דוחות עבור הסורק</span><span class="sxs-lookup"><span data-stu-id="31263-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="31263-120">סקירת התיעוד של Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="31263-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="31263-121">דרישות עבור Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="31263-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="31263-122">הורד את לקוח Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="31263-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
