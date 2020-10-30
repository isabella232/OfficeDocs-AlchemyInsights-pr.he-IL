---
title: מחבר מקומי של Exchange של כוונון האתר
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807648"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="924df-102">מחבר מקומי של Exchange של כוונון האתר</span><span class="sxs-lookup"><span data-stu-id="924df-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="924df-103">לקבלת פרטים על הגדרת המחבר בין המנגינה לבין Exchange המתארח באופן מקומי, עיין בתיעוד הבא:</span><span class="sxs-lookup"><span data-stu-id="924df-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="924df-104">הגדרת מחבר Exchange המקומי ב-Microsoft intune בתכלת של Microsoft</span><span class="sxs-lookup"><span data-stu-id="924df-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="924df-105">**שאלות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="924df-105">**FAQ:**</span></span>

<span data-ttu-id="924df-106">ש: אני רואה שגיאה כגון "גירסת מחבר Exchange אינה נתמכת" בעת ניסיון להגדיר את מחבר Exchange.</span><span class="sxs-lookup"><span data-stu-id="924df-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="924df-107">מה עשויה להיות הסיבה?</span><span class="sxs-lookup"><span data-stu-id="924df-107">What could be the cause?</span></span>

<span data-ttu-id="924df-108">ת: החשבון שבו אתה משתמש מורשה כראוי-עליו לכלול רשיון של כוונון פעיל</span><span class="sxs-lookup"><span data-stu-id="924df-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="924df-109">ש: האם ניתן לכלול מחברי Exchange מרובים?</span><span class="sxs-lookup"><span data-stu-id="924df-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="924df-110">א: באפשרותך להגדיר רק מחבר Exchange אחד לכל ארגון של Exchange לכל אחד מהדיירים.</span><span class="sxs-lookup"><span data-stu-id="924df-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="924df-111">ניתן להתקין את המחבר רק בשרת אחד בארגון exchange בשרת רב-ממדי.</span><span class="sxs-lookup"><span data-stu-id="924df-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="924df-112">כמו כן, לא ניתן להגדיר מחברים שתצורתם נקבעה הן עבור Exchange Online והן של Exchange Online המוגדרות באותו דייר.</span><span class="sxs-lookup"><span data-stu-id="924df-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="924df-113">ש: האם המחבר יכול להשתמש במערך CAS כחיבור שלו ל-Exchange?</span><span class="sxs-lookup"><span data-stu-id="924df-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="924df-114">ת: ציון מערך CAS אינו תצורה נתמכת בהגדרת המחבר.</span><span class="sxs-lookup"><span data-stu-id="924df-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="924df-115">יש לציין רק שרת אחד ויש לקשיח בקובץ תצורת המחבר שניתן למצוא ב-</span><span class="sxs-lookup"><span data-stu-id="924df-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="924df-116">תוכנית data\microsoft\microsoft התכוונת למחבר Exchange המקומי \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="924df-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="924df-117">אתר את הערך הבא ```<ExchangeWebServiceURL />``` והחלף את כתובת ה-URL בשרת exchange.</span><span class="sxs-lookup"><span data-stu-id="924df-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="924df-118">**דוגמה**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="924df-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="924df-119">עיין בתיעוד הבא לאיתור בעיות נוספות: [פתרון בעיות במחבר Exchange המקומי](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="924df-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="924df-120">**הפעלת רישום Verbose עבור מחבר Exchange**</span><span class="sxs-lookup"><span data-stu-id="924df-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="924df-121">פתח את קובץ התצורה של עקיבה אחר מחבר Exchange לעריכה.</span><span class="sxs-lookup"><span data-stu-id="924df-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="924df-122">הקובץ ממוקם בכתובת: Connector\TracingConfiguration.xml%ProgramData%\Microsoft\Windows של Exchange</span><span class="sxs-lookup"><span data-stu-id="924df-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="924df-123">**דוגמה**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="924df-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="924df-124">אתר את TraceSourceLine עם המפתח הבא: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="924df-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="924df-125">שינוי ערך הצומת של SourceLevel ממידע ActivityTracing (ברירת המחדל) לActivityTracing Verbose</span><span class="sxs-lookup"><span data-stu-id="924df-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="924df-126">**דוגמה**</span><span class="sxs-lookup"><span data-stu-id="924df-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="924df-127">הפעל מחדש את שירות החליפין של Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="924df-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="924df-128">סינכרון מלא בפורטל ' כוונון ' עד שהוא מסיים ולאחר מכן שנה את ה-XML חזרה ל-"Information ActivityTracing" והפעל מחדש את שירות החליפין של Microsoft intune.</span><span class="sxs-lookup"><span data-stu-id="924df-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="924df-129">מיקום יומני הרישום הוא: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="924df-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>