---
title: ניקוי אוטומטי של התקנים ישנים בIntune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555220"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="00381-102">ניקוי אוטומטי של התקנים ישנים בIntune</span><span class="sxs-lookup"><span data-stu-id="00381-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="00381-103">Intune מאפשר למנהל לקבוע תצורה של מרווח זמן בין 90 ל-270 ימים, לאחר הסרת התקנים מיושנים מהשירות.</span><span class="sxs-lookup"><span data-stu-id="00381-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="00381-104">הגדרה זו היא ארגון רחב ומופעל פעם נכנסת לתוקף מיד.</span><span class="sxs-lookup"><span data-stu-id="00381-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="00381-105">כל ההתקנים שלא הוכנס לשרת Intune לתקופה שתעלה על ההגדרה יימחקו לצמיתות.</span><span class="sxs-lookup"><span data-stu-id="00381-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="00381-106">**שים לב** רק אובייקטי התקן MDM זכאים לפעולת ניקוי זו.</span><span class="sxs-lookup"><span data-stu-id="00381-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="00381-107">רק אובייקטים של התקן EA אינם נכללים.</span><span class="sxs-lookup"><span data-stu-id="00381-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="00381-108">לקבלת מידע נוסף אודות המועד שבו התקן הופך להיות זכאי למחיקה בהתבסס על הגדרת הניקוי של ההתקן והמצב שלו:</span><span class="sxs-lookup"><span data-stu-id="00381-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="00381-109">הגדרה: **מחיקת התקנים לאחר תאריך הצ-אין האחרון: כן (ערך מסוים (N) בימים שצוין)**</span><span class="sxs-lookup"><span data-stu-id="00381-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="00381-110">בהתבסס על הערך (N) שהוגדר בהגדרה, שירות Intune מוחק את ההתקן בימים שצוינו לאחר שהוא מבצע בהצלחה את הצ-אין.</span><span class="sxs-lookup"><span data-stu-id="00381-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="00381-111">הגדרה: **התקני מחיקה לאחר תאריך הצ-אין האחרון: No**</span><span class="sxs-lookup"><span data-stu-id="00381-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="00381-112">180 ימים לאחר תפוגת אישור ההתקן ואינו מתחדש, ההתקן נמחק.</span><span class="sxs-lookup"><span data-stu-id="00381-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="00381-113">**שים לב** בשני המקרים, יש לרשום את ההתקן בהצלחה ב-Intune.</span><span class="sxs-lookup"><span data-stu-id="00381-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="00381-114">הרישום מתרחש במהלך ההתקן הראשון הכולל את שירות Intune.</span><span class="sxs-lookup"><span data-stu-id="00381-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="00381-115">אם התקן מתגלגל בהצלחה ל-Intune אך אינו הופך לIntune רשום, ההתקן נמחק 270 ימים לאחר ההרשמה.</span><span class="sxs-lookup"><span data-stu-id="00381-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="00381-116">(90 ימים כדי לסמן את ההתקן כפי שבוטל, ולאחר מכן 180 ימים נוספים כדי למחוק את הרשומה.)</span><span class="sxs-lookup"><span data-stu-id="00381-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="00381-117">לא קיים מנגנון הנמצא כעת במסוף Intune כדי לקבוע את תאריך התפוגה של אישור ההתקן עבור כל התקן נתון.</span><span class="sxs-lookup"><span data-stu-id="00381-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>