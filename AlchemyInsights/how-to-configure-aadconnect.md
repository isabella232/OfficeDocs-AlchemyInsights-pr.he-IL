---
title: 646 כיצד להגדיר את התצורה של AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722543"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f28ba-102">קביעת תצורה של תכונות סינכרון</span><span class="sxs-lookup"><span data-stu-id="f28ba-102">Configure sync features</span></span>

<span data-ttu-id="f28ba-103">תכלת ההתחברות כוללת מספר תכונות הזמינות כברירת מחדל, או שניתן להפוך אותן לזמינות מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="f28ba-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="f28ba-104">תכונות מסוימות דורשות תצורה נוספת בסביבות ספציפיות.</span><span class="sxs-lookup"><span data-stu-id="f28ba-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="f28ba-105">[סינון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) מגביל את האובייקטים שהאובייקטים מסונכרנים לתכלת AD.</span><span class="sxs-lookup"><span data-stu-id="f28ba-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="f28ba-106">כברירת מחדל, כל המשתמשים, אנשי הקשר, הקבוצות וחשבונות המחשבים של Windows 10 מסונכרנים.</span><span class="sxs-lookup"><span data-stu-id="f28ba-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="f28ba-107">באפשרותך לכלול או לא לכלול אובייקטים המבוססים על קבוצות מחשבים, OUs או תכונות אחרות.</span><span class="sxs-lookup"><span data-stu-id="f28ba-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="f28ba-108">[סינכרון hash של סיסמה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) מסנכרן את קוד ה-hash של הסיסמה מהספריה הפעילה המקומית אל תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="f28ba-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="f28ba-109">פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש באותה סיסמה הן בסביבות מקומיות והן בסביבת ענן.</span><span class="sxs-lookup"><span data-stu-id="f28ba-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="f28ba-110">מכיוון ש-Active Directory הוא המקור הסמכותי, באפשרותך להשתמש במדיניות סיסמה משלך.</span><span class="sxs-lookup"><span data-stu-id="f28ba-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="f28ba-111">[איפוס סיסמה של שירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן הצמתים תוך שהם עדיין מיישמים את מדיניות הסיסמה המקומית.</span><span class="sxs-lookup"><span data-stu-id="f28ba-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="f28ba-112">כותב [המכשיר](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) מאפשר התקנים רשומים בתכלת AD כדי להיכתב חזרה ל-active Directory המקומי כדי שניתן יהיה להשתמש בהם עבור גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="f28ba-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="f28ba-113">[מנע מחיקות בשוגג](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) כברירת מחדל כדי לסייע במניעת מחיקות של אובייקטים בו (יותר מ-500 אובייקטים לכל סינכרון).</span><span class="sxs-lookup"><span data-stu-id="f28ba-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="f28ba-114">באפשרותך לשנות הגדרה זו כדי לענות על צרכי הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="f28ba-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="f28ba-115">[שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) מאופשר כברירת מחדל עבור התקנות מפורשת ומסייע להבטיח שגירסת ה-"כחול החיבור" שלך תהיה תמיד עדכנית.</span><span class="sxs-lookup"><span data-stu-id="f28ba-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
