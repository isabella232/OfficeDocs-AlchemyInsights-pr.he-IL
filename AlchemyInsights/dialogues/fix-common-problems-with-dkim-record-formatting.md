---
title: פתרון בעיות נפוצות בעיצוב רשומות של DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524396"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="0edf0-102">פתרון בעיות נפוצות בעיצוב רשומות של DKIM</span><span class="sxs-lookup"><span data-stu-id="0edf0-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="0edf0-103">רוב בעיות ההגדרה של DKIM קשורות לרשומות DNS שגויות.</span><span class="sxs-lookup"><span data-stu-id="0edf0-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="0edf0-104">כדי לפתור את בעיות ההגדרה של DKIM, ודא שרשומת CNAME של DKIM (**לא** רשומת TXT) מעוצבת כראוי.</span><span class="sxs-lookup"><span data-stu-id="0edf0-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="0edf0-105">לקבלת מידע נוסף, ראה [מה עליך לעשות כדי להגדיר את DKIM באופן ידני ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="0edf0-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="0edf0-106">אם אתה זקוק לעזרה בנוגע לרשומות DNS באופן כללי, ראה [יצירת רשומות dns בכל ספק אירוח dns עבור Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="0edf0-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="0edf0-107">לאחר שתיצור או תעדכן את רשומות ה-DNS שלך ב-DKIM בשירות אירוח ה-DNS עבור התחום שלך, יהיה עליך להמתין עד להפיץ את רשומות ה-DNS.</span><span class="sxs-lookup"><span data-stu-id="0edf0-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
