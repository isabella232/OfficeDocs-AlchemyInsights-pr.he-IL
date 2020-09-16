---
title: תיקון יישומי Microsoft 365 לא מצליח למצוא הודעה המשויכת לרשיונות office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747696"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="2b996-102">תיקון יישומי Microsoft 365 "לא היתה אפשרות למצוא את ההודעה" רשיונות office משויכים "</span><span class="sxs-lookup"><span data-stu-id="2b996-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="2b996-103">אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2b996-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2b996-104">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט ליישומי Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b996-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2b996-105">ראה [כתובות url וטווחי כתובות IP של Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2b996-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="2b996-106">הסר [והקצה מחדש את רשיון Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) עבור המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="2b996-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="2b996-107">פתח יישום של Office [וצא](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.</span><span class="sxs-lookup"><span data-stu-id="2b996-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="2b996-108">עבור אל Windows Settings > **חשבונות**  >  **דואר אלקטרוני & חשבונות**והסר את כל חשבונות העבודה למעט החשבון המושפע.</span><span class="sxs-lookup"><span data-stu-id="2b996-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="2b996-109">עבור אל הגדרות Windows Settings > **חשבונות**  >  **גישה לעבודה או לבית הספר**, ונתק את כל חשבונות העבודה למעט החשבון המושפע.</span><span class="sxs-lookup"><span data-stu-id="2b996-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="2b996-110">איפוס מצב ההפעלה של Office.</span><span class="sxs-lookup"><span data-stu-id="2b996-110">Reset the Office activation state.</span></span> <span data-ttu-id="2b996-111">[למד כיצד לעשות זאת](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="2b996-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="2b996-112">[היכנס](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="2b996-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="2b996-113">לקבלת פתרונות נוספים לפתרון בעיות, ראה [שגיאות מוצר ללא רשיון והפעלה ב-Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="2b996-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>