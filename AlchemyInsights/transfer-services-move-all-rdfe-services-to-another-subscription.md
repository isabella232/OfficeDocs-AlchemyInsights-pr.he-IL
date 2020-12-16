---
title: שירותי העברה-העברת כל שירותי RDFE למנוי אחר
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692044"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="3879e-102">שירותי העברה-העברת כל שירותי RDFE למנוי אחר</span><span class="sxs-lookup"><span data-stu-id="3879e-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="3879e-103">**העברת משאבים**</span><span class="sxs-lookup"><span data-stu-id="3879e-103">**Move resources**</span></span>

<span data-ttu-id="3879e-104">ניתן להעביר משאבים של תכלת לקבוצת משאבים או לקבוצת משאבים אחרת תחת אותו מנוי באמצעות הפורטל התכלת, התכלת PowerShell, התכלת CLI או ה-API של REST כדי להעביר משאבים.</span><span class="sxs-lookup"><span data-stu-id="3879e-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="3879e-105">לפני שתוכל להעביר משאבים, ראה:</span><span class="sxs-lookup"><span data-stu-id="3879e-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="3879e-106">רשימת פעולות לביצוע לפני העברת משאבים</span><span class="sxs-lookup"><span data-stu-id="3879e-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="3879e-107">שירותים שניתן להעביר</span><span class="sxs-lookup"><span data-stu-id="3879e-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3879e-108">כיצד לאמת את המעבר</span><span class="sxs-lookup"><span data-stu-id="3879e-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="3879e-109">העברת הדרכה עבור שירותים</span><span class="sxs-lookup"><span data-stu-id="3879e-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3879e-110">כדי להעביר משאבים קיימים לקבוצת משאבים או למנוי אחר, באפשרותך להשתמש ב:</span><span class="sxs-lookup"><span data-stu-id="3879e-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="3879e-111">פורטל תכלת</span><span class="sxs-lookup"><span data-stu-id="3879e-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="3879e-112">תכלת PowerShell</span><span class="sxs-lookup"><span data-stu-id="3879e-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="3879e-113">תכלת CLI</span><span class="sxs-lookup"><span data-stu-id="3879e-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="3879e-114">מסוף API</span><span class="sxs-lookup"><span data-stu-id="3879e-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="3879e-115">ערכת לימוד: [העברת משאבים של תכלת לקבוצת משאבים או למנוי אחר](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="3879e-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="3879e-116">**פתרון שגיאות באמצעות מנהל המשאבים של תכלת**</span><span class="sxs-lookup"><span data-stu-id="3879e-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="3879e-117">עיין במאמרים הבאים כדי לקבל מידע על שגיאות משותפות בפריסה של תכלת ולקבל מידע כדי לפתור אותן.</span><span class="sxs-lookup"><span data-stu-id="3879e-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="3879e-118">אם אינך מצליח למצוא את קוד השגיאה עבור שגיאת הפריסה שלך, ראה [איתור קוד שגיאה](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="3879e-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="3879e-119">פתרון בעיות של שגיאות פריסה</span><span class="sxs-lookup"><span data-stu-id="3879e-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="3879e-120">פתרון בעיות בהעברת משאבי תכלת לקבוצת משאבים או למנוי חדש</span><span class="sxs-lookup"><span data-stu-id="3879e-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="3879e-121">שים לב שאם ברצונך לשדרג את מנוי התכלת שלך, כגון מעבר ללא תשלום לתשלום לפי הצורך, יהיה עליך להמיר את המנוי שלך.</span><span class="sxs-lookup"><span data-stu-id="3879e-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="3879e-122">כדי לשדרג גירסת ניסיון ללא תשלום, ראה [שדרוג גירסת הניסיון ללא תשלום או מנוי מתאר התכלת של Microsoft לתשלום לפי-לך](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="3879e-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="3879e-123">כדי לשנות חשבון של תשלום כפי שתרצה, ראה [שינוי המנוי של ' שלמו לפי כשאתה ' להצעה אחרת](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="3879e-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="3879e-124">**כדי להוסיף או לשייך מנוי של תכלת לדייר של תכלת Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="3879e-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="3879e-125">היכנס ובחר את המנוי שבו ברצונך להשתמש [בדף ' מנויים ' בפורטל התכלת](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="3879e-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="3879e-126">בחר **Change directory**.</span><span class="sxs-lookup"><span data-stu-id="3879e-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="3879e-127">סקור את כל האזהרות שמופיעות ולאחר מכן בחר **שנה**.</span><span class="sxs-lookup"><span data-stu-id="3879e-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="3879e-128">הספריה משתנה עבור המנוי ותקבל הודעת הצלחה.</span><span class="sxs-lookup"><span data-stu-id="3879e-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="3879e-129">השתמש בבורר *הספריות* כדי לעבור אל מדריך הכתובות החדש.</span><span class="sxs-lookup"><span data-stu-id="3879e-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="3879e-130">ייתכן שיחלפו עד 10 דקות עד שהכל יופיע כראוי.</span><span class="sxs-lookup"><span data-stu-id="3879e-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="3879e-131">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="3879e-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="3879e-132">העברת הבעלות על מנוי תכלת</span><span class="sxs-lookup"><span data-stu-id="3879e-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="3879e-133">העברת משאבים לקבוצת משאבים או למנוי חדש</span><span class="sxs-lookup"><span data-stu-id="3879e-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="3879e-134">ניהול משאבים באמצעות פורטל תכלת</span><span class="sxs-lookup"><span data-stu-id="3879e-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
