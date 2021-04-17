---
title: מפתחות שחזור של Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820287"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="965df-102">גישה למפתחות שחזור של Bitlocker</span><span class="sxs-lookup"><span data-stu-id="965df-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="965df-103">בעת קביעת התצורה של הגדרות Bitlocker Intune Endpoint Protection Policy, ניתן להגדיר אם יש לאחסן מידע שחזור של Bitlocker ב- Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="965df-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="965df-104">אם הגדרה זו מוגדרת, נתוני השחזור המאוחסנים אמורים להיות גלויים למנהל Intune כחלק מנתוני הרשומה של המכשיר בלהב Intune Devices בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="965df-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="965df-105">מכשירים - מכשירי Azure AD -> "Device" OR Devices -> כל המכשירים -> "Device" -> מפתחות שחזור</span><span class="sxs-lookup"><span data-stu-id="965df-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="965df-106">לחלופין, אם ישנה גישה ניהולית למכשיר עצמו, ניתן לראות את מפתח השחזור (סיסמה) על-ידי הפעלת הפקודה הבאה משורת פקודה עם הרשאות מלאות:</span><span class="sxs-lookup"><span data-stu-id="965df-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="965df-107">אם המכשיר הוצפן לפני הרישום ב- Intune, ייתכן שמפתח השחזור משויך ל-"Microsoft Account" (MSA) ששימש כדי להיכנס למכשיר במהלך תהליך ה- OOBE.</span><span class="sxs-lookup"><span data-stu-id="965df-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="965df-108">במקרה זה, הגישה וההכניסה באמצעות MSA זה אמורים  https://onedrive.live.com/recoverykey להציג את המכשירים שעבורם אוחסנו מפתחות שחזור.</span><span class="sxs-lookup"><span data-stu-id="965df-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="965df-109">אם המכשיר היה מוצפן כתוצאה מתצורה באמצעות מדיניות קבוצתית מבוססת תחום, ייתכן שמידע השחזור יאוחסן ב- Active Directory המקומי.</span><span class="sxs-lookup"><span data-stu-id="965df-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="965df-110">אם הגדרת מדיניות הגנה על נקודת קצה לאחסון מפתח השחזור ב- Azure Active Directory, אך המפתח עבור מכשיר ספציפי לא הועלה, באפשרותך להפעיל את ההעלאה על-ידי סיבוב מפתח השחזור עבור מכשיר זה ממסוף MEM.</span><span class="sxs-lookup"><span data-stu-id="965df-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="965df-111">לקבלת פרטים, ראה [סיבוב מפתחות שחזור של BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="965df-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

