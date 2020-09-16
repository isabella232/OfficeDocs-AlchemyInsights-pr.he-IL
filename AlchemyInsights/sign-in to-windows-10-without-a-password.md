---
title: כניסה ל-Windows 10 ללא שימוש בסיסמה
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719954"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="37390-102">כניסה ל-Windows 10 ללא שימוש בסיסמה</span><span class="sxs-lookup"><span data-stu-id="37390-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="37390-103">כדי להימנע מהקלדת סיסמה ב-Windows startup, מומלץ להשתמש באחת מאפשרויות הכניסה המאובטחת של Windows שלום, כגון מספר זיהוי אישי, זיהוי פנים או טביעת אצבע, אם הם זמינים.</span><span class="sxs-lookup"><span data-stu-id="37390-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="37390-104">אם אתה בטוח שברצונך להפוך את הכניסה המאובטחת ללא זמינה, עיין בהוראות "כניסה אוטומטית ל-Windows 10" להלן.</span><span class="sxs-lookup"><span data-stu-id="37390-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="37390-105">**מאובטח חלופות של Windows שלום לסיסמה של החשבון**</span><span class="sxs-lookup"><span data-stu-id="37390-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="37390-106">עבור אל **הגדרות חשבונות > > אפשרויות כניסה** (או לחץ [כאן](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="37390-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="37390-107">אפשרויות כניסה זמינות יופיעו.</span><span class="sxs-lookup"><span data-stu-id="37390-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="37390-108">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="37390-108">For example:</span></span>

![אפשרויות כניסה.](media/sign-in-options.png)

<span data-ttu-id="37390-110">לחץ או הקש על אחת מהאפשרויות כדי לקבוע את תצורתה.</span><span class="sxs-lookup"><span data-stu-id="37390-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="37390-111">בפעם הבאה שתפעיל או תבטל את הנעילה של Windows, תוכל להשתמש באפשרות החדשה במקום בסיסמה.</span><span class="sxs-lookup"><span data-stu-id="37390-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="37390-112">**כניסה אוטומטית ל-Windows 10**</span><span class="sxs-lookup"><span data-stu-id="37390-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="37390-113">**הערה**: כניסה אוטומטית היא נוחה, אך מציגה סיכון אבטחה, במיוחד אם המחשב שלך נגיש על-ידי אנשים מרובים.</span><span class="sxs-lookup"><span data-stu-id="37390-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="37390-114">לחץ או הקש על לחצן **התחל** בשורת המשימות.</span><span class="sxs-lookup"><span data-stu-id="37390-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="37390-115">הקלד **netplwiz** ולאחר מכן הקש על מקש Enter כדי לפתוח את החלון ' חשבונות משתמשים '.</span><span class="sxs-lookup"><span data-stu-id="37390-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="37390-116">**בחשבונות משתמשים**, לחץ על החשבון שאליו ברצונך להיכנס באופן אוטומטי כאשר Windows מופעל.</span><span class="sxs-lookup"><span data-stu-id="37390-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="37390-117">בטל את הסימון בתיבת הסימון "משתמשים חייבים להזין שם משתמש וסיסמה כדי להשתמש במחשב זה".</span><span class="sxs-lookup"><span data-stu-id="37390-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![משתמשים חייבים להזין שם משתמש וסיסמה.](media/users-must-enter-username.png)

5. <span data-ttu-id="37390-119">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="37390-119">Click **OK**.</span></span> <span data-ttu-id="37390-120">תתבקש להזין ולאשר את הסיסמה עבור החשבון שבחרת.</span><span class="sxs-lookup"><span data-stu-id="37390-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="37390-121">לחץ על **אישור** כדי לסיים.</span><span class="sxs-lookup"><span data-stu-id="37390-121">Click **OK** to finish.</span></span> <span data-ttu-id="37390-122">בפעם הבאה שחלונות 10 תופעל, היא תיכנס באופן אוטומטי לחשבון שבחרת.</span><span class="sxs-lookup"><span data-stu-id="37390-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
