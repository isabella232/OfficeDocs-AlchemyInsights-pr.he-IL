---
title: בעיות הכניסה אל יישומי Office
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938230"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="bab28-102">בעיות הכניסה אל יישומי Office</span><span class="sxs-lookup"><span data-stu-id="bab28-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="bab28-103">כדי לפתור בעיות כניסה עם יישומי Office, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="bab28-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="bab28-104">הסר את כל החשבונות עבודה, מלבד חשבון המושפעת, באמצעות הגדרות Windows > **Access בעבודה או בבית הספר**.</span><span class="sxs-lookup"><span data-stu-id="bab28-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="bab28-105">[אישורי Office ניקוי](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="bab28-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="bab28-106">**הערה:** נתיבי רישום עבור Office 2016 השתנו כדי 16.0.</span><span class="sxs-lookup"><span data-stu-id="bab28-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="bab28-107">(לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="bab28-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="bab28-108">פתח את יישום Office, בחר ' **קובץ**' > **חשבון** > **התנתק**. לאחר מכן היכנס באמצעות חשבון משתמש בעל רשיון חוקי.</span><span class="sxs-lookup"><span data-stu-id="bab28-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="bab28-109">למידע מפורט, ראו [תיקי לקוחות ב- Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="bab28-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="bab28-110">עבור Mac, ראה [יכול להיכנס אל 2016 Office עבור Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="bab28-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="bab28-111">אם השגיאות מתרחשת בעת התחברות אל Office 365 באמצעות Office 2013, לאפשר אימות מודרני עבור לקוח Office.</span><span class="sxs-lookup"><span data-stu-id="bab28-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="bab28-112">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="bab28-112">For more information, see:</span></span>
- [<span data-ttu-id="bab28-113">אין באפשרותך להיכנס ל- Office 365, תכלת הרקיע או Intune</span><span class="sxs-lookup"><span data-stu-id="bab28-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="bab28-114">בעיות חיבור בהכניסה לאחר העדכון ל- Office 2016 לבנות 16.0.7967 על Windows 10</span><span class="sxs-lookup"><span data-stu-id="bab28-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="bab28-115">"מצטערים, חשבון אחר מהארגון שלך מחובר כבר במחשב זה" ב- Office</span><span class="sxs-lookup"><span data-stu-id="bab28-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="bab28-116">פתרון בעיות כניסה באמצעות אימות מודרני של Office בעת שימוש ADFS</span><span class="sxs-lookup"><span data-stu-id="bab28-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)