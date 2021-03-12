---
title: הקבוצה ' עותק משוכפל '
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714257"
---
# <a name="replica-set"></a><span data-ttu-id="9471c-102">הקבוצה ' עותק משוכפל '</span><span class="sxs-lookup"><span data-stu-id="9471c-102">Replica set</span></span>

<span data-ttu-id="9471c-103">AADDS נקרא גם התחום המנוהל.</span><span class="sxs-lookup"><span data-stu-id="9471c-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="9471c-104">למעשה, שני בקרי תחום מופעלים ומתקיימים על-ידי הקצה העורפי.</span><span class="sxs-lookup"><span data-stu-id="9471c-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="9471c-105">שני DCs כוללים DC ראשי אחד ושכפול אחד DC.</span><span class="sxs-lookup"><span data-stu-id="9471c-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="9471c-106">גיבויים ב-AADDS (תחום מנוהל) הם תהליך אוטומטי שמנוהל על-ידי פלטפורמת התכלת.</span><span class="sxs-lookup"><span data-stu-id="9471c-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="9471c-107">במקרה של בעיה בתחום המנוהל שלך, התמיכה בנושא תכלת יכולה לסייע לך בשחזור מהגיבוי.</span><span class="sxs-lookup"><span data-stu-id="9471c-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="9471c-108">אתה יוצר כל עותק משוכפל ברשת וירטואלית.</span><span class="sxs-lookup"><span data-stu-id="9471c-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="9471c-109">כל רשת וירטואלית חייבת להיות מוסדרת לכל רשת וירטואלית אחרת המארחת ערכת עותקים משוכפלים של תחום מנוהל.</span><span class="sxs-lookup"><span data-stu-id="9471c-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="9471c-110">תצורה זו יוצרת טופולוגיה של רשת שינוי שתומכת בשכפול מדריכי כתובות.</span><span class="sxs-lookup"><span data-stu-id="9471c-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="9471c-111">רשת וירטואלית יכולה לתמוך בערכות עותק משוכפל מרובות, בתנאי שכל קבוצת עותקים משוכפלים נמצאת ברשת משנה וירטואלית אחרת.</span><span class="sxs-lookup"><span data-stu-id="9471c-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="9471c-112">לקבלת פרטים נוספים על קבוצת עותקים משוכפלים, ראה [ערכות עותקים משוכפלים של מושגים](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="9471c-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
