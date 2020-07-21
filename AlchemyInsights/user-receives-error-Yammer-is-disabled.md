---
title: המשתמש מקבל שגיאה AADSTS7000112 Yammer אינו זמין
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198058"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="5274d-102">המשתמש מקבל שגיאה AADSTS7000112 Yammer אינו זמין</span><span class="sxs-lookup"><span data-stu-id="5274d-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="5274d-103">אם אתה מקבל את השגיאה "AADSTS7000112: יישום" 00000005-0000-0ff1-ce00-000000000000 ' (Yammer) אינו זמין ", קיימת בעיה עם מנהל השירות בתוך התכלת.</span><span class="sxs-lookup"><span data-stu-id="5274d-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="5274d-104">ייתכן שמנהל המערכת ביטל את מנהל השירות כדי לחסום את הגישה ליאממר.</span><span class="sxs-lookup"><span data-stu-id="5274d-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="5274d-105">השבתת מנהל השירות אינה מומלצת ויכולה לגרום לבעיות נוספות.</span><span class="sxs-lookup"><span data-stu-id="5274d-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="5274d-106">לקבלת מידע נוסף אודות הגישה הנתמכת לחסימת גישת המשתמש ליאממר, ראה [ביטול גישת yammer עבור משתמשי Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="5274d-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="5274d-107">כדי לתקן בעיה זו בפורטל התכלת ולשחזר את גישת המשתמש ליאממר:</span><span class="sxs-lookup"><span data-stu-id="5274d-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="5274d-108">פתח את הדף ' מדריך כחול פעיל ' ובחר **יישומים ארגוניים** תחת **ניהול** בחלונית הניווט השמאלית.</span><span class="sxs-lookup"><span data-stu-id="5274d-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="5274d-109">הקלד **Office 365 Yammer** בתיבת החיפוש, ובחר את שם היישום כדי לפתוח את ההגדרות.</span><span class="sxs-lookup"><span data-stu-id="5274d-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="5274d-110">בחר **מאפיינים** תחת **ניהול** בחלונית הניווט השמאלית.</span><span class="sxs-lookup"><span data-stu-id="5274d-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="5274d-111">האם להגדיר את הערך **הזמין עבור משתמשים להיכנס?** **ככן**ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="5274d-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="5274d-112">. היכנס ליאממר שוב</span><span class="sxs-lookup"><span data-stu-id="5274d-112">Sign in to Yammer again.</span></span> <span data-ttu-id="5274d-113">. אולי תצטרך לנקות את העוגיות</span><span class="sxs-lookup"><span data-stu-id="5274d-113">You might need to clear cookies.</span></span>

<span data-ttu-id="5274d-114">לחלופין, הפעל פקודות PowerShell כדי להגדיר את הערך.</span><span class="sxs-lookup"><span data-stu-id="5274d-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="5274d-115">לקבלת מידע נוסף, ראה ["מצטערים, אך אנו מתקשים לחתום על השגיאה" בעת לחיצה על האריח Yammer ב-Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="5274d-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 