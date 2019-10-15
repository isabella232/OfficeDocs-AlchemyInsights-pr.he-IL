---
title: רשימות גדולות של SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488518"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="9a4d1-102">עבודה עם רשימות וספריות גדולות ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="9a4d1-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="9a4d1-103">רשימות וספריות של SharePoint יכולות להכיל עד 30,000,000 פריטים, אך כאשר יש להם יותר מ-5,000 פריטים, ייתכן שתראה שגיאה של סף תצוגת רשימה בעת ניסיון לעבוד איתן.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="9a4d1-104">הסף הזה נמצא במקומו. כדי לשמור על ביצועי השירות</span><span class="sxs-lookup"><span data-stu-id="9a4d1-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="9a4d1-105">. אי אפשר לשנות את זה</span><span class="sxs-lookup"><span data-stu-id="9a4d1-105">It can't be changed.</span></span> <span data-ttu-id="9a4d1-106">כדי להימנע מפגיעה בהסף הזה:</span><span class="sxs-lookup"><span data-stu-id="9a4d1-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="9a4d1-107">**השתמש בסגנון מודרני**</span><span class="sxs-lookup"><span data-stu-id="9a4d1-107">**Use modern**</span></span>

<span data-ttu-id="9a4d1-108">תצוגות המציגות פריטים רבים פועלים במיטבו בחוויה המודרנית.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="9a4d1-109">[השתמש בחוויה המודרנית](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) כדי למנוע שגיאות שייתכן שתראה בחוויה הקלאסית.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="9a4d1-110">**הוספת אינדקסים**</span><span class="sxs-lookup"><span data-stu-id="9a4d1-110">**Add indexes**</span></span>

<span data-ttu-id="9a4d1-111">בעת סינון או מיון לפי עמודה שאין לה אינדקס, ייתכן שתראה הודעת שגיאה.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="9a4d1-112">הוסף אינדקס באופן ידני מתוך **הגדרות רשימה** בתפריט ההגדרות, ולאחר מכן [הוספת](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) **אינדקס לעמודות**.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="9a4d1-113">**ערוך את תצוגת הרשימה**</span><span class="sxs-lookup"><span data-stu-id="9a4d1-113">**Edit the list view**</span></span>

<span data-ttu-id="9a4d1-114">אם מתרחשת שגיאה בעת עבודה עם רשימה גדולה, [ערוך את תצוגת הרשימה](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="9a4d1-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="9a4d1-115">ארבעת השינויים הבאים יסירו שגיאות הסף לתצוגת רשימה.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="9a4d1-116">בצע את כל ארבעת השינויים כדי להסיר את כל השגיאות.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="9a4d1-117">אם אתה עדיין מקבל שגיאות, בדוק את [ניהול רשימות וספריות גדולות](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="9a4d1-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="9a4d1-118">בחר **בללא** **מהמיון הראשון לפי העמודה** **ולאחר מכן מיין לפי העמודה**.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="9a4d1-119">בחר **בללא** משתי **הקבוצות הראשונות לפי העמודה** **ולאחר מכן קבץ לפי העמודה**.</span><span class="sxs-lookup"><span data-stu-id="9a4d1-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="9a4d1-120">בחר **ללא** עבור כל העמודות במקטע **הסיכומים** .</span><span class="sxs-lookup"><span data-stu-id="9a4d1-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="9a4d1-121">בטלו את הבחירה בעמודה אחת לתצוגה ממקטע **העמודות** .</span><span class="sxs-lookup"><span data-stu-id="9a4d1-121">Deselect all but one column for display from the **Columns** section.</span></span>

