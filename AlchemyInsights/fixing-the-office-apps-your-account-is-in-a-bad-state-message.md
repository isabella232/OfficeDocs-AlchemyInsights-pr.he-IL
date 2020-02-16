---
title: תיקון יישומי Office החשבון שלך נמצא בהודעת מצב לא טובה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969495"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="b64a7-102">תיקון היישומים של Office "החשבון שלך במצב רע" שגיאה</span><span class="sxs-lookup"><span data-stu-id="b64a7-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="b64a7-103">כדי לתקן שגיאה זו, נסה את האפשרויות הבאות במחשב המושפע:</span><span class="sxs-lookup"><span data-stu-id="b64a7-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="b64a7-104">פתח יישום Office, בחר את > **החתימה של\*\*\*\*חשבון** **הקובץ** > מכל החשבונות.</span><span class="sxs-lookup"><span data-stu-id="b64a7-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="b64a7-105">היכנס שוב באמצעות חשבון משתמש עם רשיון חוקי.</span><span class="sxs-lookup"><span data-stu-id="b64a7-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="b64a7-106">לקבלת מידע מפורט, ראה [תיקי לקוחות ב-Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="b64a7-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="b64a7-107">[נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="b64a7-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="b64a7-108">**הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0.</span><span class="sxs-lookup"><span data-stu-id="b64a7-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b64a7-109">לדוגמה, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="b64a7-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="b64a7-110">במחשב המושפע, הגדר את האפשרות Enabהפניות אל = 0 באמצעות השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b64a7-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="b64a7-111">לחץ לחיצה ימנית על לחצן Windows ובחר באפשרות **הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="b64a7-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="b64a7-112">בתיבה **פתח את** , הקלד **regedit**ולאחר מכן בחר **באפשרות אישור**.</span><span class="sxs-lookup"><span data-stu-id="b64a7-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="b64a7-113">בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="b64a7-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="b64a7-114">בעורך הרישום, הוסף ערך DWORD של Enabמסוף עם הגדרה של 0 תחת HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="b64a7-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="b64a7-115">אם השגיאה מתרחשת בעת התחברות ל-Office 365 באמצעות Office 2013, [הפעל אימות מודרני](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) עבור לקוח office.</span><span class="sxs-lookup"><span data-stu-id="b64a7-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="b64a7-116">לקבלת מידע נוסף, ראה [כיצד לפתור בעיות ביישומים שאינם של הדפדפן שאינם יכולים להיכנס ל-Office 365, תכלת או Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="b64a7-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

