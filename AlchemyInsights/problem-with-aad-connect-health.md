---
title: בעיה עם האפשרות ' התחבר לתקינות '
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482067"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="0fc8c-102">בעיה עם האפשרות ' התחבר לתקינות '</span><span class="sxs-lookup"><span data-stu-id="0fc8c-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="0fc8c-103">ודא שאתה מורשה לבצע את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="0fc8c-104">למנהלי מערכת כלליים יש גישה כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-104">Global Admins have access by default.</span></span> <span data-ttu-id="0fc8c-105">בנוסף, באפשרותך להשתמש [בבקרת גישה מבוססת תפקידים](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) כדי להקצות הרשאת רישום למשתתף.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="0fc8c-106">ודא שנקודות הקצה הנדרשות זמינות, ולא נחסמות עקב חומת האש.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="0fc8c-107">לקבלת פרטים, ראה [דרישות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="0fc8c-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="0fc8c-108">הרישום עשוי להיכשל עקב תקשורת יוצאת הנתונה לפיקוח SSL על-ידי שכבת הרשת.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="0fc8c-109">ודא שאימתת את הגדרות ההודעה עבור בריאות הקישור תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="0fc8c-110">עיין בהגדרה.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-110">Please review your setting.</span></span> <span data-ttu-id="0fc8c-111">[מדריך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) זה יכול לעזור לך להבין כיצד לקבוע את התצורה של הגדרות ההודעה עבור הודעות בריאות של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="0fc8c-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="0fc8c-112">לקבלת מידע נוסף אודות דוח הסינכרון של התקינות של החיבור הרפואי של ה-עמ ואופן ההורדה שלו, ראה [דוח סינכרון ברמת האובייקט](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="0fc8c-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="0fc8c-113">כדי לפתור בעיות בחיבור של התראות תקינות, בצע [את מדריך פתרון הבעיות עבור הצגת התראות טריות של נתוני תקינות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ולגבי שאלות נפוצות, ראה האפשרות [המשותפת לגבי התקנת שאלות של התקנת תקינות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="0fc8c-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
