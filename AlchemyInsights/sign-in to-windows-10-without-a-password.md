---
title: כניסה ל- Windows 10 ללא שימוש בסיסמה
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830547"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="0ef86-102">כניסה ל- Windows 10 ללא שימוש בסיסמה</span><span class="sxs-lookup"><span data-stu-id="0ef86-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="0ef86-103">כדי להימנע מהקלדה של סיסמה בעת ההפעלה של Windows, מומלץ להשתמש באחת מאפשרויות הכניסה המאובטחות של Windows Hello, כמו מספר זיהוי אישי, זיהוי פנים או טביעת אצבע, אם היא זמינה.</span><span class="sxs-lookup"><span data-stu-id="0ef86-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="0ef86-104">אם ברצונך להפוך כניסה מאובטחת ללא זמינה, עיין בהוראות "היכנס באופן אוטומטי ל- Windows 10" להלן.</span><span class="sxs-lookup"><span data-stu-id="0ef86-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="0ef86-105">**Secure Windows Hello חלופות לסיסמאת החשבון**</span><span class="sxs-lookup"><span data-stu-id="0ef86-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="0ef86-106">עבור אל **הגדרות > חשבונות > אפשרויות כניסה** (או לחץ [כאן](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="0ef86-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="0ef86-107">אפשרויות הכניסה הזמינות יופיעו ברשימה.</span><span class="sxs-lookup"><span data-stu-id="0ef86-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="0ef86-108">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="0ef86-108">For example:</span></span>

![אפשרויות כניסה.](media/sign-in-options.png)

<span data-ttu-id="0ef86-110">לחץ או הקש על אחת מהאפשרויות כדי לקבוע את תצורתה.</span><span class="sxs-lookup"><span data-stu-id="0ef86-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="0ef86-111">בפעם הבאה שתפתח או תפתח את Windows, תוכל להשתמש באפשרות החדשה במקום בסיסמה.</span><span class="sxs-lookup"><span data-stu-id="0ef86-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="0ef86-112">**כניסה אוטומטית ל- Windows 10**</span><span class="sxs-lookup"><span data-stu-id="0ef86-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="0ef86-113">**הערה:** כניסה אוטומטית היא נוחה, אך מציגה סיכון אבטחה, במיוחד אם המחשב שלך נגיש על-ידי אנשים מרובים.</span><span class="sxs-lookup"><span data-stu-id="0ef86-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="0ef86-114">לחץ או הקש על **לחצן** התחל בשורת המשימות.</span><span class="sxs-lookup"><span data-stu-id="0ef86-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="0ef86-115">הקלד **netplwiz** ולאחר מכן הקש על מקש Enter כדי לפתוח את החלון חשבונות משתמשים.</span><span class="sxs-lookup"><span data-stu-id="0ef86-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="0ef86-116">תחת **חשבונות משתמשים,** לחץ על החשבון שברצונך להיכנס בו באופן אוטומטי בעת הפעלת Windows.</span><span class="sxs-lookup"><span data-stu-id="0ef86-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="0ef86-117">בטל את הסימון בתיבת הסימון "משתמשים חייבים להזין שם משתמש וסיסמה כדי להשתמש במחשב זה".</span><span class="sxs-lookup"><span data-stu-id="0ef86-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![המשתמשים חייבים להזין אפשרות של שם משתמש וסיסמה.](media/users-must-enter-username.png)

5. <span data-ttu-id="0ef86-119">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="0ef86-119">Click **OK**.</span></span> <span data-ttu-id="0ef86-120">תתבקש להזין ולאשר את הסיסמה עבור החשבון שבחרת.</span><span class="sxs-lookup"><span data-stu-id="0ef86-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="0ef86-121">לחץ **על אישור** כדי לסיים.</span><span class="sxs-lookup"><span data-stu-id="0ef86-121">Click **OK** to finish.</span></span> <span data-ttu-id="0ef86-122">בפעם הבאה ש- Windows 10 יופעל, הוא יירשם באופן אוטומטי לחשבון שבחרת.</span><span class="sxs-lookup"><span data-stu-id="0ef86-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
