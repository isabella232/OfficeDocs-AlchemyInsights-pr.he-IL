---
title: יצירת מדיניות תוויות של AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569202"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="80bff-102">יצירת מדיניות תוויות של AIP</span><span class="sxs-lookup"><span data-stu-id="80bff-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="80bff-103">ניתן להשתמש בתוויות הגנה מפני מידע תכלת (AIP) עם טווח הנתונים המלא שארגון בדרך כלל יוצר ומאחסן, מהסיווג הנמוך ביותר של נתונים אישיים, לסיווג הגבוה ביותר של נתונים סודיים ביותר.</span><span class="sxs-lookup"><span data-stu-id="80bff-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="80bff-104">מדיניות הגנת מידע תכלת חלה על הלקוח הקלאסי של הגנת המידע (AIP) ולא על [לקוח התיוג המאוחד של aip](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="80bff-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="80bff-105">באפשרותך להגדיר רכיבים מרובים במדיניות AIP, כולל אפשרויות כגון:</span><span class="sxs-lookup"><span data-stu-id="80bff-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="80bff-106">אפשרות עבור איזו תווית יאפשר למנהלי מערכת או לסווג משתמש והגנה (אופציונלי) מסמכים ואימיילים</span><span class="sxs-lookup"><span data-stu-id="80bff-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="80bff-107">אפשרות לאכוף סיווג כאשר משתמשים שומרים מסמכים ושולחים דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="80bff-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="80bff-108">אפשרות לתייג באופן אוטומטי הודעת דואר אלקטרוני, בהתבסס על הקבצים המצורפים שלה.</span><span class="sxs-lookup"><span data-stu-id="80bff-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="80bff-109">אפשרות לקביעה אם סרגל הגנת המידע מוצג ביישומי Office</span><span class="sxs-lookup"><span data-stu-id="80bff-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="80bff-110">למידע נוסף על מדיניות הגנת המידע בתכלת, ראו: [מבט כולל על מדיניות הגנת המידע בתכלת](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="80bff-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="80bff-111">לקבלת משאבים שימושיים נוספים לגבי מדיניות AIP, ראה:</span><span class="sxs-lookup"><span data-stu-id="80bff-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="80bff-112">ערכת לימוד: קביעת תצורה של הגדרות מדיניות הגנת מידע תכלת ויצירת תווית חדשה</span><span class="sxs-lookup"><span data-stu-id="80bff-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="80bff-113">הגדרת מדיניות הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="80bff-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="80bff-114">יצירה וקביעת תצורה של תוויות רגישות והמדיניות שלהם</span><span class="sxs-lookup"><span data-stu-id="80bff-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="80bff-115">מדריכי ' כיצד לעשות ' עבור תרחישים נפוצים המשתמשים בהגנה על מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="80bff-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="80bff-116">סקירת התיעוד של הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="80bff-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="80bff-117">דרישות להגנה מפני מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="80bff-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="80bff-118">הדרכה מהירה עבור הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="80bff-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="80bff-119">הורד את לקוח הגנת מידע תכלת</span><span class="sxs-lookup"><span data-stu-id="80bff-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)