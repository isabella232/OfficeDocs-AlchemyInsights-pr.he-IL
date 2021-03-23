---
title: קביעת התצורה של נקודת חיבור שירות (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036142"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="b2121-102">קביעת התצורה של נקודת חיבור שירות (SCP)</span><span class="sxs-lookup"><span data-stu-id="b2121-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="b2121-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="b2121-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="b2121-104">**סיבה**: אין אפשרות לקרוא את האובייקט SCP ולקבל את המידע על הדייר של תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="b2121-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="b2121-105">**פתרון**: עיין בסעיף [קביעת תצורה של נקודת חיבור לשירות](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="b2121-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="b2121-106">**תוכנית פעולה**</span><span class="sxs-lookup"><span data-stu-id="b2121-106">**Action plan**</span></span>

- <span data-ttu-id="b2121-107">בדוק אם המכשיר קיבל את ה-GPO עבור האימות המבוקר.</span><span class="sxs-lookup"><span data-stu-id="b2121-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="b2121-108">ודא ש-GPO יצר את מפתחות הרישום.</span><span class="sxs-lookup"><span data-stu-id="b2121-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="b2121-109">ודא שיש לך שני מקשים שנוצרו באמצעות מזהה הספריה והתחום של onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="b2121-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="b2121-110">**קביעת התצורה של הגדרת רישום בצד הלקוח עבור SCP**</span><span class="sxs-lookup"><span data-stu-id="b2121-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="b2121-111">השתמש בדוגמה הבאה כדי ליצור אובייקט מדיניות קבוצתית (GPO) כדי לפרוס הגדרת רישום הקובעת ערך SCP ברישום של המכשירים שלך.</span><span class="sxs-lookup"><span data-stu-id="b2121-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="b2121-112">פתח מסוף ניהול מדיניות קבוצתית וצור GPO חדש בתחום שלך.</span><span class="sxs-lookup"><span data-stu-id="b2121-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="b2121-113">ספק שם לאובייקט ה-GPO החדש שיצרת (לדוגמה, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="b2121-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="b2121-114">ערוך את ה-GPO ואתר את הנתיב הבא: **תצורת מחשב > העדפות > הגדרות Windows > רישום**.</span><span class="sxs-lookup"><span data-stu-id="b2121-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="b2121-115">לחץ באמצעות לחצן העכבר הימני על **הרישום** ובחר **פריט רישום חדש >**.</span><span class="sxs-lookup"><span data-stu-id="b2121-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="b2121-116">בכרטיסיה **כללי** , קבע את תצורת הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b2121-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="b2121-117">**פעולה**: עדכון</span><span class="sxs-lookup"><span data-stu-id="b2121-117">**Action**: Update</span></span>
    
- <span data-ttu-id="b2121-118">**כוורת**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="b2121-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="b2121-119">**נתיב מפתח**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="b2121-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="b2121-120">**שם ערך**: TenantId</span><span class="sxs-lookup"><span data-stu-id="b2121-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="b2121-121">**סוג ערך**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="b2121-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="b2121-122">**נתוני ערך**: GUID או מזהה מדריך הכתובות של מופע ה-"תכלת לספירה" (ערך זה ניתן למצוא **בפורטל תכלת > תכלת active Directory > מאפיינים > מזהה מדריך כתובות**)</span><span class="sxs-lookup"><span data-stu-id="b2121-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="b2121-123">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="b2121-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="b2121-124">לחץ באמצעות לחצן העכבר הימני על **הרישום** ובחר **פריט רישום חדש >**.</span><span class="sxs-lookup"><span data-stu-id="b2121-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="b2121-125">בכרטיסיה **כללי** , קבע את תצורת הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b2121-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="b2121-126">**פעולה**: עדכון</span><span class="sxs-lookup"><span data-stu-id="b2121-126">**Action**: Update</span></span>
    
- <span data-ttu-id="b2121-127">**כוורת**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="b2121-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="b2121-128">**נתיב מפתח**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="b2121-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="b2121-129">**שם ערך**: TenantName</span><span class="sxs-lookup"><span data-stu-id="b2121-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="b2121-130">**סוג ערך**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="b2121-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="b2121-131">**נתוני ערך**: שם התחום המאומת שלך אם אתה משתמש בסביבה מאוחדת כגון AD FS.</span><span class="sxs-lookup"><span data-stu-id="b2121-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="b2121-132">שם התחום שאומת או שם התחום שלך ב-onmicrosoft.com (לדוגמה, contoso. onmicrosoft). com אם אתה משתמש בסביבה מנוהלת</span><span class="sxs-lookup"><span data-stu-id="b2121-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="b2121-133">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="b2121-133">Click **OK**.</span></span>

7. <span data-ttu-id="b2121-134">סגור את העורך עבור ה-GPO החדש שנוצר.</span><span class="sxs-lookup"><span data-stu-id="b2121-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="b2121-135">קשר את ה-GPO החדש שנוצר לקבוצה הרצויה של OU המכילה מחשבים המצורפים לתחום השייכים לאוכלוסיית הפריסה הנשלטת.</span><span class="sxs-lookup"><span data-stu-id="b2121-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="b2121-136">לקבלת מידע נוסף, ראה [אימות מבוקר של הצטרפות כלאיים של תכלת-תכלת לספירה | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [ופתרון בעיות היברידית תכלת active Directory הצטרפו למכשירים | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="b2121-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









