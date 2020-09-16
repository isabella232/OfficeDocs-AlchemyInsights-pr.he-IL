---
title: תיקון יישומי Microsoft 365 החשבון שלך מופיע בהודעת מצב רע
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744546"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="7c95e-102">תיקון יישומי Microsoft 365 "החשבון שלך נמצא במצב גרוע"</span><span class="sxs-lookup"><span data-stu-id="7c95e-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="7c95e-103">כדי לתקן שגיאה זו, נסה את האפשרויות הבאות במחשב המושפע:</span><span class="sxs-lookup"><span data-stu-id="7c95e-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="7c95e-104">פתח יישום של Office, בחר **File**באפשרות  >  **Account**  >  **כניסה לחשבון קובץ מכל החשבונות**.</span><span class="sxs-lookup"><span data-stu-id="7c95e-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="7c95e-105">היכנס שוב באמצעות חשבון משתמש עם רשיון חוקי.</span><span class="sxs-lookup"><span data-stu-id="7c95e-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="7c95e-106">לקבלת מידע, ראה [חשבונות ב- Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="7c95e-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="7c95e-107">[נקה את אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="7c95e-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="7c95e-108">**הערה:** נתיבי הרישום של Office 2016 השתנו ל-16.0.</span><span class="sxs-lookup"><span data-stu-id="7c95e-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7c95e-109">לדוגמה, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="7c95e-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="7c95e-110">אם השגיאה מתרחשת בעת ההתחברות ל-Office 365 באמצעות Office 2013, [הפוך אימות מודרני לזמין](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) עבור לקוח Office.</span><span class="sxs-lookup"><span data-stu-id="7c95e-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="7c95e-111">לקבלת מידע נוסף, ראה [כיצד לפתור בעיות יישומים שאינם משתמשים בדפדפנים שאינם מצליחים להיכנס ל-Microsoft 365, לתכלת או למנגינה](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="7c95e-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

