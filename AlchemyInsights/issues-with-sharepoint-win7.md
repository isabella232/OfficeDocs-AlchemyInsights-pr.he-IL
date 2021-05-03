---
title: בעיות עם SharePoint ב- Windows 7 מחשבים
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125121"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="a220d-102">בעיות עם SharePoint ב- Windows 7 מחשבים</span><span class="sxs-lookup"><span data-stu-id="a220d-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="a220d-103">אם אתה מקבל שגיאות ב- Windows 7 מחשבים במהלך העבודה על SharePoint או OneDrive, ייתכן שהן קשורות לפחת של TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="a220d-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="a220d-104">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="a220d-104">For more information, see:</span></span>

- [<span data-ttu-id="a220d-105">הכנה ל-TLS 1.2 ב-Office 365 ו-Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="a220d-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="a220d-106">Windows 7 SP1/Windows 8 לקוחות צריכים להיות זמינים ב- TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="a220d-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="a220d-107">לקבלת מידע נוסף, [ראה שגיאות אימות מתרחשות כאשר ללקוח אין תמיכה ב- TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="a220d-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="a220d-108">התקן את KB3140245 וצור את ערך הרישום.</span><span class="sxs-lookup"><span data-stu-id="a220d-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="a220d-109">לקבלת מידע נוסף, ראה [עדכון כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows</span><span class="sxs-lookup"><span data-stu-id="a220d-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="a220d-110">Windows 7 SP1/Windows 8 חייבים לוודא שסוויטות הצופן העדכניות ביותר של TLS מותקנות.</span><span class="sxs-lookup"><span data-stu-id="a220d-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="a220d-111">לקבלת מידע נוסף, ראה [עלון יידוע בנושא אבטחה של Microsoft מס' 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="a220d-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


