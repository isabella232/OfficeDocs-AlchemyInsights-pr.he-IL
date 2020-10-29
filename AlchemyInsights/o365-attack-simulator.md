---
title: סימולטור התקפה של 2681 ב-Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801552"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="d1b19-102">סימולטור התקפה ב-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d1b19-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="d1b19-103">האם חסר לך סימולטור התקפה?</span><span class="sxs-lookup"><span data-stu-id="d1b19-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="d1b19-104">סימולטור **התקפה דורש Microsoft Defender עבור office 365 תוכנית 2 (ATP תוכנית 2)** או **Office 365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="d1b19-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="d1b19-105">סימולטור התקפה **אינו** כלול ב-Microsoft Defender עבור Office 365 תוכנית 1 (ATP Plan 1), Office 365 Enterprise E3, או כל אפליקציות Microsoft 365 למנויים עסקיים.</span><span class="sxs-lookup"><span data-stu-id="d1b19-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="d1b19-106">החשבון שבו אתה משתמש להפעלת התקפות מדומה דורש הרשאות מנהל מערכת כללי או מנהל אבטחה ואימות רב-גורמי.</span><span class="sxs-lookup"><span data-stu-id="d1b19-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="d1b19-107">לקבלת מידע נוסף אודות דרישות סימולטור התקפה, עיין [בנושא זה](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="d1b19-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="d1b19-108">דברים חשובים שעליך לדעת על סימולציות התקפה **בסיסמאות של כוח פיזי** :</span><span class="sxs-lookup"><span data-stu-id="d1b19-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="d1b19-109">אם חשבון היעד הזמין את משרד המשתמש והסיסמה התמלאה כראוי, החשבון לא יוצג כסכנה (מקדם האימות השני לא יהיה שלם).</span><span class="sxs-lookup"><span data-stu-id="d1b19-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="d1b19-110">קובץ הסיסמה אינו יכול להיות גדול מ-10 MB.</span><span class="sxs-lookup"><span data-stu-id="d1b19-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="d1b19-111">השתמש בסיסמה אחת בכל שורה וכלול שורה ריקה (החזרת גררה) לאחר הסיסמה האחרונה ברשימה.</span><span class="sxs-lookup"><span data-stu-id="d1b19-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="d1b19-112">דברים חשובים שעליך לדעת לגבי הדמיית **החנית** מצרף סימולציות:</span><span class="sxs-lookup"><span data-stu-id="d1b19-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="d1b19-113">לפי עיצוב, אין באפשרותך לספק ערך מותאם אישית עבור **כתובת URL של שרת הכניסה לדיוג** .</span><span class="sxs-lookup"><span data-stu-id="d1b19-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="d1b19-114">אם נמען משתמש [בתוספת הפיכת הודעת הדוח לזמינה](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) כדי לדווח על ההודעה כדיוג, ייתכן שלא תקבל התראות עבור ההודעה (מכיוון שזוהי התקפה מדומה).</span><span class="sxs-lookup"><span data-stu-id="d1b19-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="d1b19-115">דוחות: לאחר השלמת ההתקפה המדומה, באפשרותך ללחוץ על **פרטי התקפה** כדי לראות את הדוח.</span><span class="sxs-lookup"><span data-stu-id="d1b19-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="d1b19-116">לקבלת הוראות מפורטות ותכונות חדשות בסימולטור התקפה, ראה [סימולטור התקפה ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="d1b19-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
