---
title: 401 שגיאה לא מורשית SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233499"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="eabb9-102">401 שגיאה לא מורשית SharePoint</span><span class="sxs-lookup"><span data-stu-id="eabb9-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="eabb9-103">אם אתה מקבל את השגיאה "(401) לא מורשה" ב- SharePoint ייתכן שהיא קשורה לפחת של TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="eabb9-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="eabb9-104">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="eabb9-104">For more info, see:</span></span>

[<span data-ttu-id="eabb9-105">הכנה ל-TLS 1.2 ב-Office 365 ו-Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="eabb9-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="eabb9-106">שגיאות אימות מתרחשות אם ללקוח אין תמיכה ב- TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="eabb9-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="eabb9-107">אם המשתמשים נמצאים ב- Windows 7, ודא שהם בודקים [את TLS Cipher Suites ב- Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="eabb9-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>