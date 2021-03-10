---
title: דוגמה של Microsoft Defender עבור מדיניות האנטי-דיוג של Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694037"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="ad94e-102">דוגמה של Microsoft Defender עבור מדיניות האנטי-דיוג של Office 365</span><span class="sxs-lookup"><span data-stu-id="ad94e-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="ad94e-103">הגדרות אלה מאפשרות מדיניות הנקראת *Domain ו-מנכ*.</span><span class="sxs-lookup"><span data-stu-id="ad94e-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="ad94e-104">מדיניות זו מספקת גם הגנה על משתמשים ותחומים מפני התחזות ולאחר מכן מחילה את המדיניות על כל הדואר האלקטרוני שהתקבלו על-ידי משתמשים בתוך התחום.</span><span class="sxs-lookup"><span data-stu-id="ad94e-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="ad94e-105">תחילה, הוסף את המידע הבא כדי ליצור את המדיניות:</span><span class="sxs-lookup"><span data-stu-id="ad94e-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="ad94e-106">**שם**: תחום **ותיאור** מנכ: מבטיח שהמנכ המנכ והתחום שלך לא יתבצעו התחזות.</span><span class="sxs-lookup"><span data-stu-id="ad94e-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="ad94e-107">**הוחל** על: בחר **את תחום הנמען**.</span><span class="sxs-lookup"><span data-stu-id="ad94e-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="ad94e-108">תחת **אחת מהאפשרויות הבאות**, בחר **באפשרות בחר** ולאחר מכן בחר תחום.</span><span class="sxs-lookup"><span data-stu-id="ad94e-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="ad94e-109">בחר **+ Add**.</span><span class="sxs-lookup"><span data-stu-id="ad94e-109">Select **+ Add**.</span></span> <span data-ttu-id="ad94e-110">בחר את תיבת הסימון לצד שם התחום ברשימה (לדוגמה, *contoso.com*) ולאחר מכן בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="ad94e-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="ad94e-111">בחר **ביצוע**.</span><span class="sxs-lookup"><span data-stu-id="ad94e-111">Select **Done**.</span></span>
- <span data-ttu-id="ad94e-112">לאחר יצירת המדיניות, באפשרותך לכוונן את המדיניות באמצעות האפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ad94e-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="ad94e-113">**הוסף משתמשים להגנה:** בדוגמה זו, הוסף את כתובת הדואר האלקטרוני של המנכ, לכל הפחות.</span><span class="sxs-lookup"><span data-stu-id="ad94e-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="ad94e-114">**הוסף תחומים להגנה**: הוסף את התחום הארגוני הכולל את office של המנכ.</span><span class="sxs-lookup"><span data-stu-id="ad94e-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="ad94e-115">**בחר פעולות**: אם הודעת **דואר אלקטרוני נשלחת על-ידי משתמש מתחזה**, בחר באפשרות **ניתוב מחדש של הודעה לכתובת דואר אלקטרוני אחרת** ולאחר מכן הזן את כתובת הדואר האלקטרוני של מנהל האבטחה (לדוגמה, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="ad94e-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="ad94e-116">אם הודעת **דואר אלקטרוני נשלחת על-ידי תחום מתחזה**, בחר **הסגר את ההודעה**.</span><span class="sxs-lookup"><span data-stu-id="ad94e-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="ad94e-117">**מודיעין תיבת דואר**: כברירת מחדל, אפשרות זו נבחרת בעת יצירת מדיניות חדשה למניעת דיוג.</span><span class="sxs-lookup"><span data-stu-id="ad94e-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="ad94e-118">השאר הגדרה זו **מופעלת** לקבלת התוצאות הטובות ביותר.</span><span class="sxs-lookup"><span data-stu-id="ad94e-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="ad94e-119">**הוסף שולחים ותחומים מהימנים:** עבור דוגמה זו, אל תגדיר דריסות.</span><span class="sxs-lookup"><span data-stu-id="ad94e-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="ad94e-120">לאחר שתסקור את ההגדרות, בחר **צור מדיניות זו** או **שמור**, בהתאם לצורך.</span><span class="sxs-lookup"><span data-stu-id="ad94e-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="ad94e-121">לקבלת מידע נוסף, ראה [מדיניות למניעת דיוג ב-Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="ad94e-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
