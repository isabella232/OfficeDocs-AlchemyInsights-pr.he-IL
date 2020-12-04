---
title: שימוש בתוכניות בסיסיות אבטחה של Microsoft לקביעת התצורה של מכשירי Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573398"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="9ff97-102">שימוש בתוכניות בסיסיות אבטחה של Microsoft לקביעת התצורה של מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="9ff97-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="9ff97-103">כוונון תוכניות בסיסיות של אבטחה, עזור להגן על משתמשים ומכשירים.</span><span class="sxs-lookup"><span data-stu-id="9ff97-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="9ff97-104">תוכניות בסיסיות של אבטחה הן קבוצות המוגדרות מראש של הגדרות Windows המשמשות להחלת קבוצה ידועה של הגדרות וערכי ברירת מחדל המומלצים על-ידי צוותי האבטחה הרלוונטיים.</span><span class="sxs-lookup"><span data-stu-id="9ff97-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="9ff97-105">על-ידי יצירת פרופיל תוכנית בסיסית של אבטחה ב-intune, עליך ליצור תבנית המורכבת מפרופילים מרובים של תצורת התקן.</span><span class="sxs-lookup"><span data-stu-id="9ff97-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="9ff97-106">בעת פריסת תוכניות בסיסיות של אבטחה לקבוצות של משתמשים או מכשירים, ההגדרות מוחלות על מכשירים הפועלים ב-Windows 10 ואילך.</span><span class="sxs-lookup"><span data-stu-id="9ff97-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="9ff97-107">לדוגמה, תוכנית הבסיס לאבטחה של MDM באופן אוטומטי (1) מאפשרת ל-BitLocker עבור כוננים נשלפים (2) לדרוש את הסיסמה לנעילת התקן, ו-(3) הפיכת אימות בסיסי ללא זמין.</span><span class="sxs-lookup"><span data-stu-id="9ff97-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="9ff97-108">כאשר ערך ברירת מחדל אינו פועל עבור הסביבה שלך, התאם אישית את תוכנית הבסיס כדי להחיל את ההגדרות הדרושות.</span><span class="sxs-lookup"><span data-stu-id="9ff97-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="9ff97-109">תוכניות בסיסיות של אבטחה עוזרות גם ליצור זרימת עבודה מאובטחת מקצה לקצה ב-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ff97-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="9ff97-110">להלן היתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="9ff97-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="9ff97-111">תוכנית בסיסית של אבטחה כוללת את שיטות העבודה המומלצות וההמלצות עבור הגדרות המשפיעות על האבטחה.</span><span class="sxs-lookup"><span data-stu-id="9ff97-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="9ff97-112">מכיוון ש-intune שותפים עם צוות האבטחה של Windows שיוצר תוכניות בסיסיות עבור פריטי מדיניות קבוצתית, המלצות אלה מבוססות על הדרכה מוצקה וניסיון רב.</span><span class="sxs-lookup"><span data-stu-id="9ff97-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="9ff97-113">אם אתה משתמש חדש ב-intune ואינך בטוח היכן להתחיל, בסיסי אבטחה יסייע לך ליצור ולפרוס במהירות פרופיל מאובטח.</span><span class="sxs-lookup"><span data-stu-id="9ff97-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="9ff97-114">אם אתה משתמש כעת במדיניות קבוצתית, ולאחר מכן העברה למטרת השימוש ב-intune למטרות ניהול היא קלה הרבה יותר באמצעות תוכניות בסיסיות של אבטחה, מכיוון שהן מוכללות בתוך המנגינה וכוללות יכולות גזירה לניהול.</span><span class="sxs-lookup"><span data-stu-id="9ff97-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="9ff97-115">לקבלת מידע נוסף, ראה [בסיסי אבטחה של Windows](https://go.microsoft.com/fwlink/?linkid=2141503) [וניהול מכשירים ניידים](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="9ff97-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>