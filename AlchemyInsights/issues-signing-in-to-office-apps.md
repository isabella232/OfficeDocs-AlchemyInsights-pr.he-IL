---
title: בעיות בכניסה לאפליקציות Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833076"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="6db59-102">הודעת תיקון אפליקציות Microsoft 365 "מצטערים, חשבון אחר מהארגון שלך כבר מחובר"</span><span class="sxs-lookup"><span data-stu-id="6db59-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="6db59-103">כדי לתקן שגיאה זו, נסה את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="6db59-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="6db59-104">הסר את כל חשבונות העבודה, למעט החשבון המושפע, באמצעות הגדרות Windows > **Access בעבודה או בבית ספר**.</span><span class="sxs-lookup"><span data-stu-id="6db59-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="6db59-105">[נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="6db59-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6db59-106">**הערה:** נתיבי הרישום עבור Office 2016 השתנו ל- 16.0.</span><span class="sxs-lookup"><span data-stu-id="6db59-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6db59-107">(לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6db59-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="6db59-108">פתח יישום של Office, בחר  >  **'צא**  >  **מחשב קובץ'.** לאחר מכן היכנס באמצעות חשבון משתמש עם רשיון חוקי.</span><span class="sxs-lookup"><span data-stu-id="6db59-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="6db59-109">לקבלת מידע, ראה [חשבונות ב- Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="6db59-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="6db59-110">עבור Mac, ראה [לא ניתן להיכנס לאפליקציית Office 2016 עבור Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="6db59-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="6db59-111">לקבלת מידע נוסף, [ראה "מצטערים, חשבון אחר מהארגון](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)שלך כבר מחובר במחשב זה" ב- Office.</span><span class="sxs-lookup"><span data-stu-id="6db59-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>