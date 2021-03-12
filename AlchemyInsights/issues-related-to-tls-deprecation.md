---
title: אין אפשרות לשלוח/לקבל דואר אלקטרוני אל/מ-Office 365 בשל היכולת של TLS 1.0 ו-TLS 1.1
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
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745017"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="40aac-102">אין אפשרות לשלוח/לקבל דואר אלקטרוני אל/מ-Office 365 בשל היכולת של TLS 1.0 ו-TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="40aac-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="40aac-103">כפי שאושר על-ידי מרכז ההודעות של post MC229914, TLS 1.0 ו-TLS 1.1 תבטלות התחיל לאכוף נקודות קצה של זרימת דואר מקוונת של Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="40aac-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="40aac-104">בקרוב, Office 365 לא יקבל עוד חיבורי הדואר האלקטרוני של TLS 1.0 ו-TLS 1.1 ממקורות חיצוניים.</span><span class="sxs-lookup"><span data-stu-id="40aac-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="40aac-105">בנוסף, Exchange Online לעולם לא ישתמש ב-TLS 1.0 או ב-1.1 כדי לשלוח דואר אלקטרוני יוצא.</span><span class="sxs-lookup"><span data-stu-id="40aac-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="40aac-106">אם אתה עומד בפני בעיות עקב היכולת של TLS 1.0 או 1.1, ייתכן שתיתקל באחת מהשגיאות הבאות-</span><span class="sxs-lookup"><span data-stu-id="40aac-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="40aac-107">השולח מקבל החזרה משלוח באמצעות NDR-' 421 החיבור של 4.4.2 צנח עקב SocketError '</span><span class="sxs-lookup"><span data-stu-id="40aac-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="40aac-108">שגיאה במציג התורים של שרת מקומי ששולח דואר אלקטרוני לשוטר 365-' 421 4.4.2 ' התנתק עקב SocketError '</span><span class="sxs-lookup"><span data-stu-id="40aac-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="40aac-109">שגיאה [ביומן](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) שליחת פרוטוקול מחבר בשרת שולח דואר אלקטרוני אל Office 365-משאים ומתנים של TLS נכשלו עם שגיאה SocketError</span><span class="sxs-lookup"><span data-stu-id="40aac-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="40aac-110">שגיאה ביומן השליחה או הקבלה של פרוטוקול מחבר-' 451 5.7.3 חייב להנפיק את הפקודה STARTTLS תחילה '</span><span class="sxs-lookup"><span data-stu-id="40aac-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="40aac-111">אם אתה נתקל בשגיאות שלעיל, ודא שהשרת ששולח או מקבל דואר אלקטרוני מכיל את האפשרות TLS 1.2 מופעל על-ידי בדיקת מפתחות הרישום הבאים-</span><span class="sxs-lookup"><span data-stu-id="40aac-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="40aac-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ לקוח] **"DisabledByDefault" = dword: 00000000 "Enabled" = dword: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = dword: 00000000 "זמין" = dword: 00000001**</span><span class="sxs-lookup"><span data-stu-id="40aac-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="40aac-113">אם תבצע שינוי כלשהו במפתחות הרישום לעיל כדי להפוך את TLS 1.2 לזמין, הפעל מחדש את השרת כדי שהשינויים ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="40aac-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="40aac-114">כמו כן, ודא שהתקנת את העדכונים האחרונים של Windows ו-Exchange.</span><span class="sxs-lookup"><span data-stu-id="40aac-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="40aac-115">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="40aac-115">For more information, see:</span></span>

- [<span data-ttu-id="40aac-116">הדרכה של Exchange Server TLS, חלק 1: התכונן לקבלת TLS 1.2-קהילת Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="40aac-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="40aac-117">חלק הדרכה של Exchange Server TLS 2: הפעלת TLS 1.2 וזיהוי לקוחות שאינם משתמשים בה-קהילת Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="40aac-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="40aac-118">הכרת תרחישי דואר אלקטרוני אם לא ניתן להסכים על גירסאות TLS באמצעות Exchange Online-קהילת Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="40aac-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
