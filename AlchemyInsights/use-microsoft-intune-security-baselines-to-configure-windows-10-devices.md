---
title: שימוש בתוכניות הבסיסיות של האבטחה Microsoft intune לקביעת התצורה של מכשירי Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694432"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="c4c3d-102">שימוש בתוכניות בסיסיות האבטחה של Microsoft intune לקביעת התצורה של מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="c4c3d-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="c4c3d-103">כוונון תוכניות בסיסיות של אבטחה, עזור להגן על משתמשים ומכשירים.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="c4c3d-104">תוכניות בסיסיות של אבטחה הן קבוצות המוגדרות מראש של הגדרות Windows המשמשות להחלת קבוצה ידועה של הגדרות וערכי ברירת מחדל המומלצים על-ידי צוותי האבטחה הרלוונטיים.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="c4c3d-105">על-ידי יצירת פרופיל תוכנית בסיסית של אבטחה ב-intune, עליך ליצור תבנית המורכבת מפרופילים מרובים של תצורת התקן.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="c4c3d-106">בעת פריסת תוכניות בסיסיות של אבטחה לקבוצות של משתמשים או מכשירים, ההגדרות מוחלות על מכשירים הפועלים ב-Windows 10 וגירסאות מתקדמות יותר.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="c4c3d-107">לדוגמה, התוכנית הבסיסית של ' ניהול מכשירים ניידים של Microsoft ' (MDM) באופן אוטומטי (1) מאפשרת ל-BitLocker עבור כוננים נשלפים (2) לחייב את הסיסמה לבטל נעילה של התקן ו-(3) הפיכת אימות בסיסי ללא זמין.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="c4c3d-108">כאשר ערך ברירת מחדל אינו פועל עבור הסביבה שלך, באפשרותך להתאים אישית את תוכנית הבסיס כדי להחיל את ההגדרות הדרושות.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="c4c3d-109">תוכניות בסיסיות של אבטחה עוזרות גם ליצור זרימת עבודה מאובטחת מקצה לקצה ב-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="c4c3d-110">להלן כמה מהיתרונות של פונקציונליות זו:</span><span class="sxs-lookup"><span data-stu-id="c4c3d-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="c4c3d-111">תוכנית בסיסית של אבטחה כוללת את שיטות העבודה המומלצות וההמלצות עבור הגדרות המשפיעות על האבטחה.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="c4c3d-112">מכיוון ש-intune שותפים עם צוות האבטחה של Windows שיוצר תוכניות בסיסיות עבור פריטי מדיניות קבוצתית, המלצות אלה מבוססות על הדרכה מוצקה וניסיון רב.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="c4c3d-113">אם אתה משתמש חדש ב-intune ואינך בטוח היכן להתחיל, בסיסי אבטחה יסייע לך ליצור ולפרוס במהירות פרופיל מאובטח.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="c4c3d-114">אם אתה משתמש כעת במדיניות קבוצתית, ולאחר מכן העברתם למטרות של התכוונות לניהול היא קלה הרבה יותר באמצעות תוכניות בסיסיות של אבטחה, מאחר שתוכניות בסיסיות אבטחה אלה מובנות לתוך התכתבות וכוללות יכולות גזירה לניהול.</span><span class="sxs-lookup"><span data-stu-id="c4c3d-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="c4c3d-115">לקבלת מידע נוסף, ראה [בסיסי אבטחה של Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [וניהול מכשירים ניידים](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="c4c3d-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>