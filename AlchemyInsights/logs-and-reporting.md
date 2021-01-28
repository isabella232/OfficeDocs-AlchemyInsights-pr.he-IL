---
title: יומני רישום ודיווח
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035916"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="7c2bd-102">יומני רישום ודיווח</span><span class="sxs-lookup"><span data-stu-id="7c2bd-102">Logs and Reporting</span></span>

<span data-ttu-id="7c2bd-103">[שאלות נפוצות אודות דיווח של מדריכי כתובות של Active directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) תשובות לשאלות נפוצות אודות הדיווח על תכלת Active Directory (תכלת לספירה).</span><span class="sxs-lookup"><span data-stu-id="7c2bd-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="7c2bd-104">לקבלת מידע נוסף, ראה [התכונה ' דיווח על Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)'.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="7c2bd-105">**פתרון בעיות באמצעות ביקורת**</span><span class="sxs-lookup"><span data-stu-id="7c2bd-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="7c2bd-106">אם אתה נתקל בבעיות במהלך הצגת פעילויות ביקורת והפעילות החסרה נמצאת [ברשימה](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)זו, הקובץ כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="7c2bd-107">אם אתה נתקל בבעיות בצפייה ביומני ביקורת בדייר שלך, הקובץ כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="7c2bd-108">אם פעילויות הביקורת שלך אינן מוצגות באופן מיידי בפורטל התכלת, עיין [במידע ההשהיה](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) שלנו ותייק כרטיס תמיכה אם ההשהיה חורגת מההשהיה המתועדת.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="7c2bd-109">שמירה על יומני פעילות של תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="7c2bd-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="7c2bd-110">אם אינך רואה את כל ביקורת עבור טווח התאריכים שבחרת, באפשרותך להוריד עד 250 אלף שורות (ממוינים לפי האחרונים) של כניסה מפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="7c2bd-111">לקבלת מידע נוסף, ראה [הורדת פעילויות ביקורת](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="7c2bd-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="7c2bd-112">**פתרון בעיות עם כניסה**</span><span class="sxs-lookup"><span data-stu-id="7c2bd-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="7c2bd-113">באפשרותך לראות רק את 30 הימים האחרונים של הנתונים אם יש לך רשיון תכלת AD Premium (P1 או P2) עבור הדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="7c2bd-114">הכניסה זמינה רק עבור דיירים של תכלת AD Premium.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="7c2bd-115">האפשרות אינה זמינה עבור דיירים בעלי רשיון בחינם או בסיסיים.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="7c2bd-116">אם הדייר שלך כולל רשיון מסוג Premium של P1 ואינך רואה את הכניסה, עיין [במידע ההשהיה](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) שלנו ותייק כרטיס תמיכה אם ההשהיה חורגת מההשהיה המתועדת.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="7c2bd-117">אם אינך רואה את כל הכניסה עבור טווח התאריכים שבחרת, שים לב שניתן להוריד עד 250 אלף שורות (ממוינים לפי העדכניים ביותר) של כניסה מפורטל תכלת.</span><span class="sxs-lookup"><span data-stu-id="7c2bd-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="7c2bd-118">לקבלת מידע נוסף, ראה [הורדת פעילויות של כניסה](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="7c2bd-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="7c2bd-119">**פתרון בעיות בדוחות אבטחה (משתמשים מסומנים בדגל בסיכון, כניסה מסוכנת)**</span><span class="sxs-lookup"><span data-stu-id="7c2bd-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="7c2bd-120">משתמשים המסומנים בדגל עבור דוח אבטחה של סיכון</span><span class="sxs-lookup"><span data-stu-id="7c2bd-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="7c2bd-121">דוח כניסה מסוכן בפורטל תכלת Active Directory</span><span class="sxs-lookup"><span data-stu-id="7c2bd-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="7c2bd-122">אירועי סיכון של ' תכלת Active Directory '</span><span class="sxs-lookup"><span data-stu-id="7c2bd-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
