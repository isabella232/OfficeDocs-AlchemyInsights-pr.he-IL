---
title: 2681 Attack Simulator ב- Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545727"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="75846-102">Attack Simulator ב- Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="75846-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="75846-103">האם חסר לך Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="75846-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="75846-104">Attack Simulator דורש **ש- Microsoft Defender Office 365 תוכנית 2** **או Office 365 Enterprise E5.**</span><span class="sxs-lookup"><span data-stu-id="75846-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="75846-105">Attack Simulator **אינו כלול** ב- Microsoft Defender עבור Office 365 1, Office 365 Enterprise E3 או כל יישומי Microsoft 365 לעסקים מנויים.</span><span class="sxs-lookup"><span data-stu-id="75846-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="75846-106">החשבון המשמש להפעלת התקפות מדומה דורש הרשאות כלליות של מנהל מערכת או מנהל אבטחה ואימות רב-גורמי (MFA).</span><span class="sxs-lookup"><span data-stu-id="75846-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="75846-107">לקבלת מידע נוסף אודות דרישות Attack Simulator, עיין [בנושא זה](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="75846-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="75846-108">דברים חשובים שיש לדעת על **סימולציות התקפה של** סיסמה בכוח גס:</span><span class="sxs-lookup"><span data-stu-id="75846-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="75846-109">אם חשבון היעד כולל MFA זמין והסיסמה ניחשה כראוי, החשבון לא יופיע כחשוף לסכנה (גורם האימות השני לא יהיה שלם).</span><span class="sxs-lookup"><span data-stu-id="75846-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="75846-110">קובץ הסיסמה לא יכול להיות גדול מ- 10 MB.</span><span class="sxs-lookup"><span data-stu-id="75846-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="75846-111">השתמש בסיסמה אחת בכל שורה וכלול שורה ריקה (החזרת גררה) לאחר הסיסמה האחרונה ברשימה.</span><span class="sxs-lookup"><span data-stu-id="75846-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="75846-112">דברים חשובים שיש לדעת על **ספירת דיוג מצרפים** הדמיות:</span><span class="sxs-lookup"><span data-stu-id="75846-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="75846-113">כברירת מחדל, לא ניתן לספק ערך מותאם אישית עבור כתובת URL **של שרת כניסה של דיוג**.</span><span class="sxs-lookup"><span data-stu-id="75846-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="75846-114">אם נמען [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) משתמש התוספת הפוך את התוספת 'הודעת דוח' לזמינה הדוח ההודעה כדיווג, ייתכן שלא תקבל התראות עבור ההודעה (מאחר זוהי התקפה מדומה).</span><span class="sxs-lookup"><span data-stu-id="75846-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="75846-115">דוחות: לאחר השלמת התקיפה המדומה, באפשרותך ללחוץ על פרטי **התקפה** כדי לראות את הדוח.</span><span class="sxs-lookup"><span data-stu-id="75846-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="75846-116">לקבלת הוראות מפורטות ותכונות חדשות בסימולטור התקפה, ראה [סימולטור התקפה Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="75846-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
