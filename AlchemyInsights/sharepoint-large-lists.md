---
title: רשימות גדולות של SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720134"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="23f18-102">עבודה עם רשימות וספריות גדולות ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="23f18-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="23f18-103">רשימות וספריות של SharePoint יכולות להכיל עד 30,000,000 פריטים, אך כאשר יש להם יותר מ-5,000 פריטים, ייתכן שתראה שגיאת סף תצוגת רשימה כאשר אתה מנסה לעבוד איתם.</span><span class="sxs-lookup"><span data-stu-id="23f18-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="23f18-104">סף זה נקבע כדי לשמור על ביצועי השירות.</span><span class="sxs-lookup"><span data-stu-id="23f18-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="23f18-105">לא ניתן לשנות אותו.</span><span class="sxs-lookup"><span data-stu-id="23f18-105">It can't be changed.</span></span> <span data-ttu-id="23f18-106">כדי להימנע מפגיעה במפתן זה:</span><span class="sxs-lookup"><span data-stu-id="23f18-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="23f18-107">**שימוש במודרני**</span><span class="sxs-lookup"><span data-stu-id="23f18-107">**Use modern**</span></span>

<span data-ttu-id="23f18-108">תצוגות המציגות פריטים רבים פועלים בצורה הטובה ביותר בחוויה המודרנית.</span><span class="sxs-lookup"><span data-stu-id="23f18-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="23f18-109">[השתמש בחוויה המודרנית](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) כדי למנוע שגיאות שאתה עשוי לראות בחוויה הקלאסית.</span><span class="sxs-lookup"><span data-stu-id="23f18-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="23f18-110">**הוספת אינדקסים**</span><span class="sxs-lookup"><span data-stu-id="23f18-110">**Add indexes**</span></span>

<span data-ttu-id="23f18-111">בעת סינון או מיון לפי עמודה שאינה כוללת אינדקס, ייתכן שתראה הודעת שגיאה.</span><span class="sxs-lookup"><span data-stu-id="23f18-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="23f18-112">[הוסף אינדקס](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) באופן ידני מתוך ' **הגדרות רשימה** ' בתפריט ' הגדרות ' ולאחר מכן **עמודות סדורות באינדקס**.</span><span class="sxs-lookup"><span data-stu-id="23f18-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="23f18-113">**עריכת תצוגת הרשימה**</span><span class="sxs-lookup"><span data-stu-id="23f18-113">**Edit the list view**</span></span>

<span data-ttu-id="23f18-114">אם מתרחשת שגיאה בעת עבודה עם רשימה גדולה, [ערוך את תצוגת הרשימה](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="23f18-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="23f18-115">ארבעת השינויים הבאים יסיר שגיאות סף של תצוגת רשימה.</span><span class="sxs-lookup"><span data-stu-id="23f18-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="23f18-116">בצע את כל ארבעת השינויים כדי להסיר את כל השגיאות.</span><span class="sxs-lookup"><span data-stu-id="23f18-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="23f18-117">אם אתה עדיין מקבל שגיאות, סמן את [ניהול רשימות וספריות גדולות](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="23f18-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="23f18-118">בחר **None** באפשרות ללא **מסוג ' מיון ראשון ' לפי העמודה** **ולאחר מכן מיין לפי העמודה**.</span><span class="sxs-lookup"><span data-stu-id="23f18-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="23f18-119">בחר **None** באפשרות ללא **מהקבוצה הראשונה בעמודה** **ולאחר מכן קבץ לפי העמודה**.</span><span class="sxs-lookup"><span data-stu-id="23f18-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="23f18-120">בחר **ללא** עבור כל העמודות במקטע **סכומים** .</span><span class="sxs-lookup"><span data-stu-id="23f18-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="23f18-121">בטל את הבחירה באפשרות הכל פרט לעמודה אחת לתצוגה מהמקטע **עמודות** .</span><span class="sxs-lookup"><span data-stu-id="23f18-121">Deselect all but one column for display from the **Columns** section.</span></span>

