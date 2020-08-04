---
title: Intune Wi-Fi פרופילים
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555310"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="70ca4-102">Intune Wi-Fi פרופילים</span><span class="sxs-lookup"><span data-stu-id="70ca4-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="70ca4-103">יישום מוצלח של קישוריות Wi-Fi עבור לקוחות MDM תלוי בפרופיל שנפרס כראוי, המשקף את הדרישות של תשתית ה-Wi-Fi הארגונית.</span><span class="sxs-lookup"><span data-stu-id="70ca4-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="70ca4-104">כדי לסקור את ההגדרות המתאימות עבור פלטפורמות הלקוח שאתה חוקר, ראה:</span><span class="sxs-lookup"><span data-stu-id="70ca4-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="70ca4-105">הוסף הגדרות Wi-Fi עבור התקנים המפעילים אנדרואיד ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="70ca4-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="70ca4-106">הוספת Wi-Fi הגדרות עבור אנדרואיד ארגוני ייעודי התקנים מנוהלים באופן מלא ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="70ca4-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="70ca4-107">הוספת הגדרות Wi-Fi עבור התקני iOS ו-iPadOS ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="70ca4-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="70ca4-108">הוסף הגדרות Wi-Fi עבור Windows 10 והתקנים מאוחרים יותר ב-Intune</span><span class="sxs-lookup"><span data-stu-id="70ca4-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="70ca4-109">יבא הגדרות Wi-Fi עבור התקני Windows ב-Intune</span><span class="sxs-lookup"><span data-stu-id="70ca4-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="70ca4-110">**סוגיות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="70ca4-110">**Common Issues**</span></span>

<span data-ttu-id="70ca4-111">**אני פורס פרופיל Wi-Fi התלוי באישור שנפרס שצוין בפרופיל Wi-Fi. עם זאת, פרופילי התצורה מציגים מצב שגיאה.**</span><span class="sxs-lookup"><span data-stu-id="70ca4-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="70ca4-112">בדוק שההתקן שלך קיבל את האישור.</span><span class="sxs-lookup"><span data-stu-id="70ca4-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="70ca4-113">בIntune, עבור אל **כל ההתקנים** ובחר את **תצורת**ההתקן של התקן _ gt_.</span><span class="sxs-lookup"><span data-stu-id="70ca4-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="70ca4-114">ודא שכל הפרופילים הצפויים מפורטים ונמצאים במצב מוצלח.</span><span class="sxs-lookup"><span data-stu-id="70ca4-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="70ca4-115">עבור פרופיל דמוי אדם, אם יש לך אישורי ביניים בשרשרת האישורים, ודא שהם פרוסים להתקני Android.</span><span class="sxs-lookup"><span data-stu-id="70ca4-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="70ca4-116">כדי לבדוק את מצב האישור, עבור אל פרופילי **תצורת התקן**  >  **Profiles**  >  **אנדרואיד מאפייני CA בינוניים**  >  **Properties**  >  **אישור מהימן**.</span><span class="sxs-lookup"><span data-stu-id="70ca4-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="70ca4-117">אם תמשיך לראות שגיאות, סקור את ההליכים ואת מקטעי פתרון התקלות.</span><span class="sxs-lookup"><span data-stu-id="70ca4-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="70ca4-118">לקבלת מידע נוסף, ראה [סקירה עבור פתרון בעיות של פרופילי אישורים מסוימים של SCEP באמצעות Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="70ca4-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="70ca4-119">**הפרסתי פרופיל Wi-Fi למכשיר. Intune מראה שהיא הצליחה, אך ההתקן אינו מתחבר ל-Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="70ca4-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="70ca4-120">מצב מוצלח פירושו שIntune בהצלחה את הפרופיל כפי שהוגדר.</span><span class="sxs-lookup"><span data-stu-id="70ca4-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="70ca4-121">עם זאת, ייתכן שתצורות אלה לא יתאימו לדרישות הרשת ו/או האימות שלך.</span><span class="sxs-lookup"><span data-stu-id="70ca4-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="70ca4-122">לקבלת פרטים נוספים אודות ניסיון החיבור, סקור יומני רישום בתשתית ובשירות האימות (בבקר נקודת גישה לאינטרנט אלחוטי ובשרת NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="70ca4-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="70ca4-123">ייתכן שיהיה עליך לעבוד עם צוות תשתית הרשת, או בספק ה-Wi-Fi של הספק החיצוני, כדי לאסוף ולסקור יומני רישום.</span><span class="sxs-lookup"><span data-stu-id="70ca4-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>