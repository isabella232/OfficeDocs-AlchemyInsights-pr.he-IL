---
title: התחברות עם הודעה ל-עמ
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036111"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="30d78-102">התחברות עם הודעה ל-עמ</span><span class="sxs-lookup"><span data-stu-id="30d78-102">Notification AAD Connect</span></span>

- <span data-ttu-id="30d78-103">ודא שאתה מורשה לבצע את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="30d78-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="30d78-104">למנהלי מערכת כלליים יש גישה כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="30d78-104">Global Admins have access by default.</span></span> <span data-ttu-id="30d78-105">בנוסף, באפשרותך להשתמש [בבקרת גישה מבוססת תפקידים](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) כדי להקצות הרשאת רישום למשתתף.</span><span class="sxs-lookup"><span data-stu-id="30d78-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="30d78-106">ודא שנקודות הקצה הנדרשות זמינות, ולא נחסמות עקב חומת האש.</span><span class="sxs-lookup"><span data-stu-id="30d78-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="30d78-107">לקבלת פרטים, ראה [דרישות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="30d78-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="30d78-108">הרישום עשוי להיכשל עקב תקשורת יוצאת הנתונה לפיקוח SSL על-ידי שכבת הרשת.</span><span class="sxs-lookup"><span data-stu-id="30d78-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="30d78-109">ודא שאימתת את הגדרות ההודעה עבור תכלת AD Connect בריאות וסקור את ההגדרה.</span><span class="sxs-lookup"><span data-stu-id="30d78-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="30d78-110">כדי להבין כיצד לקבוע את התצורה של הגדרות ההודעות עבור הודעות בריאות של תכלת לחבר, ראה [מדריך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)זה.</span><span class="sxs-lookup"><span data-stu-id="30d78-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="30d78-111">לקבלת מידע נוסף אודות דוח הסינכרון של התקינות של החיבור הרפואי של ה-עמ ואופן ההורדה שלו, ראה [דוח סינכרון ברמת האובייקט](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="30d78-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="30d78-112">כדי לפתור בעיות בנושא הפעלת התראות בריאות, פעל על-ידי [מדריך פתרון הבעיות עבור הצגת התראות טריות של נתוני תקינות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ושאלות נפוצות, ראה מספר הודעות ה- [עמ-משותף מחברות שאלות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="30d78-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
