---
title: צמצם את הבעיה היישום לא אותר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810485"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="28adf-102">צמצם את הבעיה "היישום לא אותר"</span><span class="sxs-lookup"><span data-stu-id="28adf-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="28adf-103">שגיאת התקנת היישום, "היישום לא אותר לאחר שההתקנה הושלמה בהצלחה", שדווחה על-ידי Intune, עשויה להופיע בכל פלטפורמות מערכות ההפעלה המרכזיות (Windows, iOS ו- Android).</span><span class="sxs-lookup"><span data-stu-id="28adf-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="28adf-104">התרחישים הנפוצים ביותר שמפיקים שגיאה זו כוללים:</span><span class="sxs-lookup"><span data-stu-id="28adf-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="28adf-105">האפליקציה עודכנה מחוץ ל- Intune (מחנות יישומים של ספקים חיצוניים) לאחר הפריסה הראשונית.</span><span class="sxs-lookup"><span data-stu-id="28adf-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="28adf-106">לדוגמה, יישומים מסוימים, כגון Google Chrome, יכולים לבצע עדכונים אוטומטיים.</span><span class="sxs-lookup"><span data-stu-id="28adf-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="28adf-107">משתמש הסיר את התקנת היישום לאחר ההתקנה הראשונית.</span><span class="sxs-lookup"><span data-stu-id="28adf-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="28adf-108">כדי לצמצם את הבעיה, תחילה בצע סקירה של המכשירים המושפעים כדי לקבוע את התרחיש שבו מתרחשת השגיאה.</span><span class="sxs-lookup"><span data-stu-id="28adf-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="28adf-109">אם היישום עודכן מחוץ ל- Intune, ניתן להגדיר את פריסת היישום כך שתתעלם מהגירסה של היישום.</span><span class="sxs-lookup"><span data-stu-id="28adf-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="28adf-110">כדי לעשות זאת, תחת **'תצורת היישום' > 'מידע על היישום'**, קבע את התכונה **'התעלם מגירסת היישום'** ל **'כן'**.</span><span class="sxs-lookup"><span data-stu-id="28adf-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="28adf-111">כאשר היעד הוא הלקוח, מומלץ להגדיר את היישום כ"נדרש", ולוודא שנפרסת הגירסה העדכנית ביותר.</span><span class="sxs-lookup"><span data-stu-id="28adf-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="28adf-112">לחלופין, בפלטפורמת iOS, ניתן להשתמש בפונקציונליות **AutoUpdate** המשויכת לתוכנית הרכישה בכמות גדולה, אשר את תצורתה ניתן לקבוע לעדכון אוטומטי לגירסאות יישומים חדשות כאשר הן הופכות לזמינות.</span><span class="sxs-lookup"><span data-stu-id="28adf-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="28adf-113">לקבלת מידע נוסף על פתרון בעיות בהתקנת יישומים, ראה [פתרון בעיות בהתקנת יישומים](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="28adf-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
