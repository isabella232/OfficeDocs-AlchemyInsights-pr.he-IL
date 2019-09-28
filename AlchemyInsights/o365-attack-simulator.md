---
title: 2681 סימולטור התקפה ב-Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305333"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="4e571-102">סימולטור התקפה ב-Office 365</span><span class="sxs-lookup"><span data-stu-id="4e571-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="4e571-103">? אתה מפספס את סימולטור התקיפה</span><span class="sxs-lookup"><span data-stu-id="4e571-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="4e571-104">סימולטור **התקפה דורש office 365 הגנה מתקדמת איום תוכנית 2 (תוכנית ATP 2)** או **Office 365 הארגון E5**.</span><span class="sxs-lookup"><span data-stu-id="4e571-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="4e571-105">סימולטור התקפה **אינו** כלול בתוכנית הגנת האיום המתקדמת של office 365 1 (תוכנית ATP 1), Office 365 Enterprise E3, או כל מנוי עסקי של office 365.</span><span class="sxs-lookup"><span data-stu-id="4e571-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="4e571-106">החשבון שאתה משתמש בו להפעלת התקפות מדומים דורש מנהל מערכת כללי או הרשאות מנהל אבטחה ואימות מרובה גורמים (משרד המרכז).</span><span class="sxs-lookup"><span data-stu-id="4e571-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="4e571-107">לקבלת מידע נוסף על דרישות סימולטור התקפה, עיין [בנושא זה](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="4e571-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="4e571-108">דברים חשובים לדעת על סימולציות התקפה **באמצעות סיסמה בכח** :</span><span class="sxs-lookup"><span data-stu-id="4e571-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="4e571-109">אם לחשבון היעד מופעל משרד המשנה והסיסמה היתה מכוונת כראוי, החשבון לא יוצג כחשוד (מקדם האימות השני לא יהיה שלם).</span><span class="sxs-lookup"><span data-stu-id="4e571-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="4e571-110">קובץ הסיסמה אינו יכול להיות גדול מ-10 MB.</span><span class="sxs-lookup"><span data-stu-id="4e571-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="4e571-111">השתמש בסיסמה אחת לכל שורה וכלול שורה ריקה (החזרת גררה) לאחר הסיסמה האחרונה ברשימה.</span><span class="sxs-lookup"><span data-stu-id="4e571-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="4e571-112">חשוב לדעת אודות **החנית** הדמיות חיבור של דיוג:</span><span class="sxs-lookup"><span data-stu-id="4e571-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="4e571-113">באמצעות עיצוב, אין באפשרותך לספק ערך מותאם אישית עבור **כתובת URL של שרת ההתחברות לדיוג**.</span><span class="sxs-lookup"><span data-stu-id="4e571-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="4e571-114">אם נמען משתמש [בתוספת הפעלת הודעת דוח](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) כדי לדווח על ההודעה כדיוג, ייתכן שלא תקבל התראות עבור ההודעה (מכיוון שזוהי התקפה מדומה).</span><span class="sxs-lookup"><span data-stu-id="4e571-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="4e571-115">דוחות: לאחר השלמת ההתקפה הדומה, באפשרותך ללחוץ על **פרטי התקפה** כדי לראות את הדוח.</span><span class="sxs-lookup"><span data-stu-id="4e571-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="4e571-116">לקבלת הוראות מפורטות ותכונות חדשות ב סימולטור התקפה, ראה [סימולטור התקפה ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="4e571-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
