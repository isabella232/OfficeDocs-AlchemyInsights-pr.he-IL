---
title: היכנס ל-Windows 10 מבלי להשתמש בסיסמה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588282"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="f6c38-102">היכנס ל-Windows 10 מבלי להשתמש בסיסמה</span><span class="sxs-lookup"><span data-stu-id="f6c38-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="f6c38-103">כדי להימנע מהקלדת סיסמה בהפעלה של Windows, מומלץ שתשתמש באחת מאפשרויות הכניסה המאובטחות של Windows שלום, כגון PIN, זיהוי פנים או טביעת אצבע, אם הן זמינות.</span><span class="sxs-lookup"><span data-stu-id="f6c38-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="f6c38-104">אם באמת ברצונך להפוך את הכניסה המאובטחת ללא זמינה, עיין בהוראות "הכניסה אוטומטית ל-Windows 10" להלן.</span><span class="sxs-lookup"><span data-stu-id="f6c38-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="f6c38-105">**אבטחת Windows שלום חלופות לסיסמת החשבון**</span><span class="sxs-lookup"><span data-stu-id="f6c38-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="f6c38-106">עבור אל **הגדרות האפשרויות הרצויות** (או לחץ [כאן](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="f6c38-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f6c38-107">אפשרויות הכניסה הזמינות יפורטו.</span><span class="sxs-lookup"><span data-stu-id="f6c38-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="f6c38-108">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="f6c38-108">For example:</span></span>

![אפשרויות כניסה.](media/sign-in-options.png)

<span data-ttu-id="f6c38-110">לחץ או הקש על אחת האפשרויות כדי לקבוע את תצורתה.</span><span class="sxs-lookup"><span data-stu-id="f6c38-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="f6c38-111">בפעם הבאה שתפעיל או תשחרר את Windows, תוכל להשתמש באפשרות החדשה במקום בסיסמה.</span><span class="sxs-lookup"><span data-stu-id="f6c38-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="f6c38-112">**הרשמה אוטומטית ל-Windows 10**</span><span class="sxs-lookup"><span data-stu-id="f6c38-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="f6c38-113">**הערה**: כניסה אוטומטית היא נוחה, אך מציגה סיכון אבטחה, במיוחד אם המחשב שלך נגיש על-ידי אנשים מרובים.</span><span class="sxs-lookup"><span data-stu-id="f6c38-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="f6c38-114">לחץ או הקש על לחצן **התחל** בשורת המשימות.</span><span class="sxs-lookup"><span data-stu-id="f6c38-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="f6c38-115">הקלד **netplwiz** ולחץ על מקש Enter כדי לפתוח את החלון חשבונות משתמשים.</span><span class="sxs-lookup"><span data-stu-id="f6c38-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="f6c38-116">**בחשבונות משתמשים**, לחץ על החשבון שאליו ברצונך להיכנס באופן אוטומטי כאשר Windows מופעל.</span><span class="sxs-lookup"><span data-stu-id="f6c38-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="f6c38-117">בטל את סימון הסימון "משתמשים חייבים להזין שם משתמש וסיסמה כדי להשתמש במחשב זה".</span><span class="sxs-lookup"><span data-stu-id="f6c38-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![משתמשים חייבים להזין שם משתמש וסיסמה.](media/users-must-enter-username.png)

5. <span data-ttu-id="f6c38-119">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="f6c38-119">Click **OK**.</span></span> <span data-ttu-id="f6c38-120">תתבקש להזין ולאשר את הסיסמה עבור החשבון שבחרת.</span><span class="sxs-lookup"><span data-stu-id="f6c38-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="f6c38-121">לחץ על **אישור** כדי לסיים.</span><span class="sxs-lookup"><span data-stu-id="f6c38-121">Click **OK** to finish.</span></span> <span data-ttu-id="f6c38-122">בפעם הבאה בה Windows 10 מופעל, הוא יכנס אוטומטית לחשבון שבחרת.</span><span class="sxs-lookup"><span data-stu-id="f6c38-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
