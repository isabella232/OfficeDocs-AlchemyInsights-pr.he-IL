---
title: משהה עדכונים מתוזמנים
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555508"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="8bba1-102">משהה עדכונים מתוזמנים</span><span class="sxs-lookup"><span data-stu-id="8bba1-102">Pausing scheduled updates</span></span>

<span data-ttu-id="8bba1-103">כאשר מונפק פקודת השהיה, ההתקנים אינם מעבדים את הפקודה עד לפעם הבאה שהם מIntune.</span><span class="sxs-lookup"><span data-stu-id="8bba1-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="8bba1-104">עקב כך, ייתכן שההתקנים שלך יהיו:</span><span class="sxs-lookup"><span data-stu-id="8bba1-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="8bba1-105">התקנת את העדכונים המתוזמנים לפני ביצוע הצ-אין.</span><span class="sxs-lookup"><span data-stu-id="8bba1-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="8bba1-106">הופעל כאשר הנפקת את הפקודה pause.</span><span class="sxs-lookup"><span data-stu-id="8bba1-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="8bba1-107">במקרה זה, כאשר המכשירים הופעל, ייתכן שהם הורידו והתקינו את העדכונים המתוזמנים לפני הצ-אין.</span><span class="sxs-lookup"><span data-stu-id="8bba1-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>