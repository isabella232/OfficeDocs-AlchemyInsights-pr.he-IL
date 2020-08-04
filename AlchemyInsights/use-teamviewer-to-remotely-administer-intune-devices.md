---
title: השתמש ב-TeamViewer לניהול מרחוק של התקני Intune
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
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555238"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="d9ba9-102">השתמש ב-TeamViewer לניהול מרחוק של התקני Intune</span><span class="sxs-lookup"><span data-stu-id="d9ba9-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="d9ba9-103">ניתן לנהל מרחוק התקנים שמנוהלים על-ידי Intune באמצעות [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="d9ba9-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="d9ba9-104">כדי לנהל את Intune באמצעות TeamViewer, השתמש בצעדים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d9ba9-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="d9ba9-105">התחל בקבלת אישורים מ-TeamViewer כדי להגדיר את מחבר TeamViewer בIntune.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="d9ba9-106">הדבר מאפשר למנהל להזין אישורים בממשק המשתמש של מחבר TeamViewer תחת ' התקנים ', פעולה חד פעמי כדי ליצור את הקישור בין Intune לשירות TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="d9ba9-107">**חלק 1: הפעלת הפעלה באמצעות התקן מרוחק**</span><span class="sxs-lookup"><span data-stu-id="d9ba9-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="d9ba9-108">תחת **כל ההתקנים**, בחר את ההתקן שבו ברצונך להתחיל הפעלה מרוחקת.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="d9ba9-109">מתוך... \*\* עוד\*\*, בחר **הפעלה חדשה של סיוע מרחוק**.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="d9ba9-110">בחר באפשרות **כן** כדי לאשר שברצונך ליצור הפעלה מרוחקת.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="d9ba9-111">לאחר ששירות TeamViewer מקבל בקשה להפעלת הפעלה מרחוק חדשה, תוכל לראות אפשרות **להפעיל סיוע מרחוק** תחת פרטי החלונית ' מבט כולל ' (או, ' יסודות ') עבור ההתקן.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="d9ba9-112">בחר באפשרות ' **הצג עוד** ' כדי להרחיב את החלונית ולהציג את מצב הסיוע מרחוק.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="d9ba9-113">בחר באפשרות **' הפעל הפעלה מרוחקת** ' כדי ליזום את ההפעלה בצד המנהל.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="d9ba9-114">בחר להוריד את הקובץ הבינארי של TeamViewer (Windows) ובחר באפשרות **הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="d9ba9-115">**שים לב** באפשרותך להתעלם מכל דף דפדפן אינטרנט שייפתח באתר האינטרנט של TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="d9ba9-116">הודע לבקשה ליישום TeamViewer כדי לבצע שינויים בהתקן (Windows בלבד).</span><span class="sxs-lookup"><span data-stu-id="d9ba9-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="d9ba9-117">יישום TeamViewer מופעל וכולל את קוד ההפעלה כדי לאמת את החיבור עם ההתקן המרוחק.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="d9ba9-118">**חלק 2: בהתקן המיועד להפעלה מרחוק**</span><span class="sxs-lookup"><span data-stu-id="d9ba9-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="d9ba9-119">פתח את פורטל החברה של Intune.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="d9ba9-120">חפש דגל הודעה: "מנהל ה-IT מבקש שליטה בהתקן זה עבור הפעלת סיוע מרחוק" ובחר את ההודעה.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="d9ba9-121">בחר להוריד את יישום TeamViewer, או הורד את האישור של יישום TeamViewer מחנות היישומים ובחר באפשרות **הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="d9ba9-122">**שים לב** באפשרותך להתעלם מכל דף דפדפן אינטרנט שייפתח באתר האינטרנט של TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="d9ba9-123">הודע לבקשה ליישום TeamViewer כדי לבצע שינויים בהתקן (Windows בלבד).</span><span class="sxs-lookup"><span data-stu-id="d9ba9-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="d9ba9-124">יישום TeamViewer מופעל וכולל את קוד ההפעלה כדי לאמת את החיבור עם ההתקן המרוחק.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="d9ba9-125">מוקפץ שואל אם ברצונך לאפשר להפעלה להתחיל.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="d9ba9-126">**שים לב** קודי ההפעלה שהופקו על-ידי שירות TeamViewer הם שימוש חד פעמי בלבד.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="d9ba9-127">אם תאבד את החיבור, עליך:</span><span class="sxs-lookup"><span data-stu-id="d9ba9-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="d9ba9-128">סגור את המופע של יישום TeamViewer בהתקן המרוחק ובתחנת העבודה של המנהל.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="d9ba9-129">סגור את פורטל החברה בהתקן המרוחק.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="d9ba9-130">צור הפעלה חדשה של "סיוע מרחוק חדש" מפורטל המנהלה.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="d9ba9-131">פתח מחדש את פורטל החברה בהתקן המרוחק כדי לקבל את ההודעה החדשה.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="d9ba9-132">הורד ופתח את יישום TeamViewer הן בהתקן המרוחק והן בתחנת העבודה של המנהל, כבעבר.</span><span class="sxs-lookup"><span data-stu-id="d9ba9-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>