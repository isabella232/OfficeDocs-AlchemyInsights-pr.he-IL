---
title: שימוש Microsoft Intune בסיסי אבטחה כדי לקבוע את התצורה של Windows 10 התקנים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793899"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="b8903-102">שימוש Microsoft Intune בסיסי אבטחה כדי לקבוע את התצורה של Windows 10 התקנים</span><span class="sxs-lookup"><span data-stu-id="b8903-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="b8903-103">תוכניות בסיסיות של אבטחה של Intune עוזרות להגן על משתמשים ומכשירים.</span><span class="sxs-lookup"><span data-stu-id="b8903-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="b8903-104">תוכניות בסיסיות אבטחה הן Windows מוגדרות מראש של קבוצות המשמשות להחלת קבוצה ידועה של הגדרות וערכים המוגדרים כברירת מחדל המומלצים על-ידי צוותי האבטחה הרלוונטיים.</span><span class="sxs-lookup"><span data-stu-id="b8903-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="b8903-105">על-ידי יצירת פרופיל בסיסי אבטחה ב- Intune, עליך ליצור תבנית המורכבת מפרופילי תצורת מכשיר מרובים.</span><span class="sxs-lookup"><span data-stu-id="b8903-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="b8903-106">בעת פריסת תוכניות בסיסיות של אבטחה בקבוצות של משתמשים או מכשירים, ההגדרות מוחלות על מכשירים הפעלה ב- Windows 10 ואילך.</span><span class="sxs-lookup"><span data-stu-id="b8903-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="b8903-107">לדוגמה, תוכנית הבסיס של ניהול מכשירים ניידים (MDM) של Microsoft מאפשרת באופן אוטומטי BitLocker עבור כוננים נשלפים, דורשת את הסיסמה לביטול נעילה של מכשיר והופכת את האימות הבסיסי ללא זמין.</span><span class="sxs-lookup"><span data-stu-id="b8903-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="b8903-108">כאשר ערך ברירת מחדל אינו פועל עבור הסביבה שלך, באפשרותך להתאים אישית את התוכנית הבסיסית כדי להחיל את ההגדרות שאתה זקוק לה.</span><span class="sxs-lookup"><span data-stu-id="b8903-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="b8903-109">תוכניות בסיסיות של אבטחה גם עוזרות ליצור זרימת עבודה מאובטחת מ בסוף Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b8903-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="b8903-110">תוכנית בסיסית של אבטחה כוללת את שיטות העבודה המומלצות וההמלצות עבור הגדרות המשפיעות על האבטחה.</span><span class="sxs-lookup"><span data-stu-id="b8903-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="b8903-111">Intune משתפת קשר עם Windows האבטחה שמיצור תוכניות בסיסיות עבור מדיניות קבוצתית, כך שהמלצות אלה מבוססות על הדרכה מבוססת וניסיון רב.</span><span class="sxs-lookup"><span data-stu-id="b8903-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="b8903-112">אם אתה משתמש חדש ב- Intune ולא בטוח היכן להתחיל, תוכניות בסיסיות אבטחה עוזרות לך ליצור ולפרוס במהירות פרופיל מאובטח.</span><span class="sxs-lookup"><span data-stu-id="b8903-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="b8903-113">אם אתה משתמש כעת במדיניות קבוצתית, המעבר ל- Intune למטרות ניהול קל הרבה יותר עם תוכניות בסיסיות אבטחה מכיוון שהן מוכללות ב- Intune וכוללות יכולות ניהול מתקדמות.</span><span class="sxs-lookup"><span data-stu-id="b8903-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="b8903-114">כדי ללמוד עוד, [ראה Windows בסיסי אבטחה וניהול](/windows/security/threat-protection/windows-security-baselines) [מכשירים ניידים](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="b8903-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

