---
title: תפקיד ניהול זהויות מורשה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088884"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="62f97-102">תפקיד ניהול זהויות מורשה (PIM)</span><span class="sxs-lookup"><span data-stu-id="62f97-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="62f97-103">**הרשאות אינן ניתנות לאחר הפעלת תפקיד**</span><span class="sxs-lookup"><span data-stu-id="62f97-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="62f97-104">בעת הפעלת תפקיד בתחום הזיהוי המיוחס של "תכלת לספירה" (PIM), ייתכן שההפעלה לא תתבצע באופן מיידי לכל הפורטלים הדורשים את התפקיד המורשה.</span><span class="sxs-lookup"><span data-stu-id="62f97-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="62f97-105">לעתים, גם אם השינוי מופץ, האחסון במטמון באינטרנט בפורטל עלול לגרום לשינוי שאינו נכנס לתוקף באופן מיידי.</span><span class="sxs-lookup"><span data-stu-id="62f97-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="62f97-106">אם ההפעלה שלך מושהית, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="62f97-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="62f97-107">צא מפורטל התכלת ולאחר מכן היכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="62f97-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="62f97-108">כאשר אתה מפעיל תפקיד תכלת או תפקיד משאב תכלת, תראה את שלבי ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="62f97-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="62f97-109">לאחר השלמת כל השלבים, תראה את הקישור ' יציאה '.</span><span class="sxs-lookup"><span data-stu-id="62f97-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="62f97-110">באפשרותך להשתמש בקישור זה כדי לצאת מהמערכת. פעולה זו תפתור את רוב המקרים עבור עיכוב הפעלה.</span><span class="sxs-lookup"><span data-stu-id="62f97-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="62f97-111">ב-PIM, ודא שאתה מופיע כחבר בתפקיד.</span><span class="sxs-lookup"><span data-stu-id="62f97-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="62f97-112">אם אתה מפעיל את תפקיד מנהל Exchange, הקפד לצאת מהמערכת ולהיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="62f97-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="62f97-113">אם הבעיה נמשכת, פתח כרטיס תמיכה והגדל זאת כבעיה.</span><span class="sxs-lookup"><span data-stu-id="62f97-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="62f97-114">אם אתה משתמש בתפקיד מנהל Exchange כדי לגשת למרכז האבטחה והתאימות, ראה השלב הבא.</span><span class="sxs-lookup"><span data-stu-id="62f97-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="62f97-115">אם אתה מפעיל תפקיד כדי לגשת למרכז האבטחה והתאימות או אם אתה מפעיל את תפקיד מנהל המערכת של SharePoint, תיתקל בעיכוב הפעלה מספר דקות עד למספר שעות.</span><span class="sxs-lookup"><span data-stu-id="62f97-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="62f97-116">זוהי בעיה ידועה, ואנו פועלים באופן פעיל עם צוותים אלה כדי לפתור את הבעיה בהקדם האפשרי.</span><span class="sxs-lookup"><span data-stu-id="62f97-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="62f97-117">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="62f97-117">For more information, see:</span></span>

- [<span data-ttu-id="62f97-118">הפעלת תפקידי המודע של ' תכלת ' ב-PIM</span><span class="sxs-lookup"><span data-stu-id="62f97-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="62f97-119">הפעלת תפקידי המשאב ' תכלת ' ב-PIM</span><span class="sxs-lookup"><span data-stu-id="62f97-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="62f97-120">**הרשאות אינן מוסרות לאחר ביטול הפעלה של תפקיד או שתוקף הפעלת התפקיד פג**</span><span class="sxs-lookup"><span data-stu-id="62f97-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="62f97-121">כאשר אתה מבטל הפעלה של תפקיד בניהול זהויות מורשה של תכלת לספירה או כאשר פג תוקפו של תקופת הפעלת תפקידים, ייתכן שיהיה עיכוב במקום שבו אתה ממשיך לקבל גישה.</span><span class="sxs-lookup"><span data-stu-id="62f97-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="62f97-122">אם הפעלת הביטול מושהית, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="62f97-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="62f97-123">אם אתה מבטל את ההפעלה של תפקיד מנהל המערכת של Exchange או שתוקפו של תקופת הפעלת התפקיד פג, ואתה מבחין בעיכוב משמעותי לפני הסרת ההרשאות, פתח כרטיס תמיכה והודע למהנדס התמיכה שלך לעזור לך לתייק כרטיס באמצעות צוות ניהול הגישה המיוחסת בתוך Office לגבי בעיה</span><span class="sxs-lookup"><span data-stu-id="62f97-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="62f97-124">אם תוקפה של תקופת ההפעלה פג, אך עדיין יש לך את הפעלת הדפדפן פתוחה, סגור את הדפדפן.</span><span class="sxs-lookup"><span data-stu-id="62f97-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="62f97-125">באפשרותך להמשיך להשתמש בתפקיד עד שתסגור הפעלה זו.</span><span class="sxs-lookup"><span data-stu-id="62f97-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="62f97-126">זוהי בעיה ידועה ואנו מביטים בתיקון אפשרי כדי לבטל באופן פעיל כל הפעלה לאחר שפג תוקפה של ההפעלה.</span><span class="sxs-lookup"><span data-stu-id="62f97-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="62f97-127">אם ההשהיה שלך שונה משני תרחישים אלה, פתח כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="62f97-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
