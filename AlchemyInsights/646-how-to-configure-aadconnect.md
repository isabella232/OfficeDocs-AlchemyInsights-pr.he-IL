---
title: 646 כיצד להגדיר AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291930"
---
# <a name="configure-sync-features"></a><span data-ttu-id="61017-102">קביעת תצורה של תכונות סינכרון</span><span class="sxs-lookup"><span data-stu-id="61017-102">Configure sync features</span></span>

<span data-ttu-id="61017-p101">התחבר AD תכלת הרקיע כולל מספר תכונות אשר מופעלות כברירת מחדל, או שבאפשרותך להפוך לזמינות במועד מאוחר יותר. תכונות מסוימות דורשות קביעת תצורה נוספת בסביבות מסוימות.</span><span class="sxs-lookup"><span data-stu-id="61017-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="61017-p102">מגבלות [סינון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) האובייקטים יסונכרנו AD תכלת הרקיע. כברירת מחדל, כל המשתמשים, אנשי קשר, קבוצות, Windows 10 חשבונות מחשב מסונכרנים. באפשרותך לכלול או לא לכלול אובייקטים לפי תחומים, יחידות ארגוניות או תכונות אחרות.</span><span class="sxs-lookup"><span data-stu-id="61017-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="61017-p103">[Syncronization ה-hash של סיסמת](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) מסנכרן hash סיסמה מ- Active Directory מקומי כדי AD תכלת הרקיע. פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש בסיסמה זהה בשני המקומית סביבות ענן. מכיוון שמקור סמכותי Active Directory, באפשרותך להשתמש מדיניות סיסמה משלך.</span><span class="sxs-lookup"><span data-stu-id="61017-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="61017-111">[איפוס סיסמה בשירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן בעת החלת מדיניות הסיסמה המקומית שלך עדיין.</span><span class="sxs-lookup"><span data-stu-id="61017-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="61017-112">[Writeback התקן](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) מאפשר ההתקנים הרשומים ב- AD תכלת הרקיע להיכתב בחזרה ל- Active Directory מקומי כך הם יכולים לשמש לקבלת גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="61017-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="61017-p104">[בטעות מנע מחיקות](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) מופעלת כברירת מחדל כדי לסייע למנוע מחיקות האובייקט בו-זמנית יותר מדי (יותר מ- 500 אובייקטים לפי סינכרון). באפשרותך לשנות הגדרה זו כדי לענות על הצרכים של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="61017-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="61017-115">[שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) מופעלת כברירת מחדל עבור התקנות מפורשת ו מסייע להבטיח שהגירסה של התחברות AD תכלת הרקיע הוא תמיד הנוכחי.</span><span class="sxs-lookup"><span data-stu-id="61017-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

