---
title: סינכרון סיסמאות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482035"
---
# <a name="password-synchronization"></a><span data-ttu-id="66f40-102">סינכרון סיסמאות</span><span class="sxs-lookup"><span data-stu-id="66f40-102">Password synchronization</span></span>

<span data-ttu-id="66f40-103">**סינכרון Hash של סיסמאות אינו פועל כלל**</span><span class="sxs-lookup"><span data-stu-id="66f40-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="66f40-104">מספר בעיות נפוצות לקוחות מתקיימים כאשר סינכרון Hash של סיסמאות אינו פועל:</span><span class="sxs-lookup"><span data-stu-id="66f40-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="66f40-105">החשבון של Active Directory המשמש את הקישור תכלת AD לתקשורת עם Active Directory מקומי אינו מקבל **שינויי שינויים במדריך** הכתובות **והשכפול של ספריות משנה את כל** ההרשאות, הנדרשות לסינכרון סיסמאות-עליך לתקן זאת על-ידי הענקת הרשאות אלה לחשבון Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66f40-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="66f40-106">סינכרון hash של סיסמאות אינו זמין לאחר שמנהל מערכת שינה את שיטת המשתמש Sign-In **מסינכרון סיסמאות** לאפשרות אחרת, כגון **איחוד עם AD FS** באשף ההתחברות של ' תכלת לספירה '-באפשרותך לפתור זאת על-ידי הפיכת התכונה ' **סינכרון hash של סיסמה** ' לזמינה באשף ההתחברות של ' תכלת ad '.</span><span class="sxs-lookup"><span data-stu-id="66f40-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="66f40-107">בעיית קישוריות עם Active Directory מקומי.</span><span class="sxs-lookup"><span data-stu-id="66f40-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="66f40-108">לדוגמה, בקרי תחומים מסוימים אינם נגישים על-ידי ' תכלת לספירה ', או [שהיציאות הנדרשות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) נחסמות על-ידי חומת האש-עליך לפתור זאת על-ידי הבטחת הקישוריות בין שרת החיבור של תכלת לספירה לבין active Directory המקומי פועלת כהלכה.</span><span class="sxs-lookup"><span data-stu-id="66f40-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="66f40-109">שרתי הקישור תכלת לספירה הנמצאת כעת במצב האחסון הזמני, שיגרום לכך שהשרת לא יוכל להשתמש בקודי hash של סיסמה-כדי לפתור את הבעיה, בצע את השלבים המתוארים בסעיף [פתרון בעיות בסינכרון סיסמאות עם סינכרון מהדורת תכלת-אין סיסמאות מסונכרנות](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="66f40-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="66f40-110">**סינכרון Hash של סיסמאות אינו פועל עבור חלק מהמשתמשים שלי**</span><span class="sxs-lookup"><span data-stu-id="66f40-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="66f40-111">אם הבחנת ש-hash של סיסמה אינו מסתנכרן עבור משתמש, השתמש במשימה **פתרון בעיות** ב-תכלת AD Connect כדי לחקור ולפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="66f40-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="66f40-112">בצע את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="66f40-112">Perform the following tasks:</span></span>

    <span data-ttu-id="66f40-113">מ.</span><span class="sxs-lookup"><span data-stu-id="66f40-113">a.</span></span> [<span data-ttu-id="66f40-114">ההפעלה של משימת פתרון הבעיה באשף</span><span class="sxs-lookup"><span data-stu-id="66f40-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="66f40-115">b.</span><span class="sxs-lookup"><span data-stu-id="66f40-115">b.</span></span> [<span data-ttu-id="66f40-116">שימוש ב-cmdlet של פתרון בעיות כדי לבדוק את בעיית סינכרון ה-hash של הסיסמה לשימוש ספציפי</span><span class="sxs-lookup"><span data-stu-id="66f40-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="66f40-117">אובייקט המשתמש המקומי של Active Directory זמין עבור **המשתמש כדי לשנות את הסיסמה באפשרות הכניסה הבאה** .</span><span class="sxs-lookup"><span data-stu-id="66f40-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="66f40-118">כאשר אפשרות זו זמינה, המשתמש מוקצה לסיסמה זמנית והוא יתבקש לשנות את הסיסמה בכניסה הבאה.</span><span class="sxs-lookup"><span data-stu-id="66f40-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="66f40-119">חיבור תכלת לספירה אינו מסנכרן סיסמאות זמניות לתכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="66f40-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="66f40-120">כדי לפתור את הבעיה לעיל, בצע אחת מהמשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="66f40-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="66f40-121">בקש מהמשתמש להיכנס ליישום מקומי (לדוגמה, שולחן העבודה של Windows) ולשנות את הסיסמה.</span><span class="sxs-lookup"><span data-stu-id="66f40-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="66f40-122">הסיסמה החדשה תסונכרן לכיוון תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="66f40-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="66f40-123">מנהל מערכת עדכן את סיסמת המשתמש מבלי להפוך את האפשרות של **משתמש לזמינה לשנות את הסיסמה בכניסה הבאה** ולשתף את הסיסמה החדשה עם המשתמש.</span><span class="sxs-lookup"><span data-stu-id="66f40-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="66f40-124">אובייקט המשתמש המקומי של Active Directory **אינו מוגדר כהלכה** עבור סינכרון אובייקטים או סינכרון סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="66f40-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="66f40-125">כדי לפתור בעיה זו, בצע את השלבים המתוארים [בסינכרון ה-hash של הסיסמה לפתרון בעיות בסינכרון של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="66f40-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







