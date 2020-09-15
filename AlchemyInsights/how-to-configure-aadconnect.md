---
title: 646 כיצד להגדיר את AADConnect
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
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704490"
---
# <a name="configure-sync-features"></a><span data-ttu-id="d1f20-102">קביעת תצורה של תכונות סינכרון</span><span class="sxs-lookup"><span data-stu-id="d1f20-102">Configure sync features</span></span>

<span data-ttu-id="d1f20-103">חיבור תכלת לספירה כולל כמה תכונות הזמינות כברירת מחדל, או שניתן להפוך אותן לזמינות במועד מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="d1f20-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="d1f20-104">תכונות מסוימות דורשות תצורה נוספת בסביבות ספציפיות.</span><span class="sxs-lookup"><span data-stu-id="d1f20-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="d1f20-105">מגבלות [סינון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) האובייקטים מסונכרנים עם התכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="d1f20-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="d1f20-106">כברירת מחדל, כל המשתמשים, אנשי הקשר, הקבוצות ו-Windows 10 חשבונות מחשב מסונכרנים.</span><span class="sxs-lookup"><span data-stu-id="d1f20-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="d1f20-107">באפשרותך לכלול או לא לכלול אובייקטים בהתבסס על תחומים, רכיבי Ou או תכונות אחרות.</span><span class="sxs-lookup"><span data-stu-id="d1f20-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="d1f20-108">[סינכרון hash של סיסמאות](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) מסנכרן את קוד ה-hash של הסיסמה ממדריך הכתובות המקומי של Active Directory לכיוון תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="d1f20-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="d1f20-109">פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש באותה סיסמה בסביבות מקומיות ובסביבת ענן.</span><span class="sxs-lookup"><span data-stu-id="d1f20-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="d1f20-110">מכיוון ש-Active Directory הוא המקור הסמכותי, באפשרותך להשתמש במדיניות הסיסמה שלך.</span><span class="sxs-lookup"><span data-stu-id="d1f20-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="d1f20-111">[איפוס סיסמה בשירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן בזמן שהם עדיין מיישמים את מדיניות הסיסמה המקומית שלך.</span><span class="sxs-lookup"><span data-stu-id="d1f20-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="d1f20-112">[התקן writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) מאפשר התקנים רשומים בתכלת AD להיכתב בחזרה אל active Directory המקומי כדי שניתן יהיה להשתמש בהם לקבלת גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="d1f20-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="d1f20-113">[מניעת מחיקה בשוגג](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) מופעלת כברירת מחדל כדי לסייע במניעת מחיקות של אובייקטים בו רבים מדי (יותר מ-500 אובייקטים לכל סינכרון).</span><span class="sxs-lookup"><span data-stu-id="d1f20-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="d1f20-114">באפשרותך לשנות הגדרה זו כדי לענות על הצרכים של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d1f20-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="d1f20-115">[שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) מופעל כברירת מחדל עבור התקנות מפורשות ומסייע להבטיח שגירסת החיבור של ' תכלת לספירה ' תהיה תמיד עדכנית.</span><span class="sxs-lookup"><span data-stu-id="d1f20-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
