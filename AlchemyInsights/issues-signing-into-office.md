---
title: בעיות בכניסה ליישומי Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763002"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="d3d08-102">בעיות בכניסה ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="d3d08-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="d3d08-103">כדי לתקן בעיות כניסה באמצעות יישומי Office, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="d3d08-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="d3d08-104">הסר את כל חשבונות העבודה, למעט החשבון המושפע, באמצעות הגדרות Windows _ **הגישה לעבודה או לבית הספר**.</span><span class="sxs-lookup"><span data-stu-id="d3d08-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="d3d08-105">[נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="d3d08-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d3d08-106">**הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0.</span><span class="sxs-lookup"><span data-stu-id="d3d08-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d3d08-107">(לשעבר: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d3d08-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d3d08-108">פתח יישום Office, בחר באפשרות ' צא**מחשבון** >  **קובץ** > **'.** לאחר מכן, היכנס באמצעות חשבון משתמש עם רשיון חוקי.</span><span class="sxs-lookup"><span data-stu-id="d3d08-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="d3d08-109">לקבלת מידע, ראה [חשבונות ב- Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="d3d08-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d3d08-110">עבור Mac, ראה [לא ניתן להיכנס לאפליקציית Office 2016 עבור Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="d3d08-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="d3d08-111">אם השגיאות מתרחשות בעת התחברות ל-Microsoft 365 באמצעות Office 2013, הפעל אימות מודרני עבור לקוח Office.</span><span class="sxs-lookup"><span data-stu-id="d3d08-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="d3d08-112">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="d3d08-112">For more information, see:</span></span>
- [<span data-ttu-id="d3d08-113">אין באפשרותך להיכנס ל-Microsoft 365, תכלת או Intune</span><span class="sxs-lookup"><span data-stu-id="d3d08-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="d3d08-114">בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 לבנות 16.0.7967 ב-Windows 10</span><span class="sxs-lookup"><span data-stu-id="d3d08-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="d3d08-115">"מצטערים, חשבון נוסף מהארגון שלך כבר מחובר למחשב זה" ב-Office</span><span class="sxs-lookup"><span data-stu-id="d3d08-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="d3d08-116">פתרון בעיות כניסה באמצעות אימות מודרני של Office בעת שימוש ב-ADFS</span><span class="sxs-lookup"><span data-stu-id="d3d08-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)