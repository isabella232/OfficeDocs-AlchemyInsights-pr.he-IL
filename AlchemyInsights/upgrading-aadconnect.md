---
title: 932 שדרוג AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806040"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="40091-102">התחברות לשדרוג תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="40091-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="40091-103">כברירת מחדל, שדרוג אוטומטי זמין עבור התחברות של תכלת לספירה, המסייעת לך להבטיח שאתה מפעיל את הגירסה העדכנית ביותר.</span><span class="sxs-lookup"><span data-stu-id="40091-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="40091-104">כדי לאמת את הגדרות השדרוג האוטומטיות, השתמש ב **-Cmdlet Get-ADSyncAutoUpgrade** ב-תכלת AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="40091-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="40091-105">ה-cmdlet יחזור לאחד מהערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="40091-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="40091-106">**זמין**: שדרוג אוטומטי מופעל.</span><span class="sxs-lookup"><span data-stu-id="40091-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="40091-107">לא **זמין**: שדרוג אוטומטי אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="40091-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="40091-108">**מושעה**: המערכת כבר אינה זכאית לקבל שדרוגים אוטומטיים.</span><span class="sxs-lookup"><span data-stu-id="40091-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="40091-109">לא ניתן לקבוע את התצורה של ערך זה; היא מוגדרת על-ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="40091-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="40091-110">לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="40091-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="40091-111">כדי להוריד את הגירסה העדכנית ביותר של תכלת AD Connect, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="40091-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
