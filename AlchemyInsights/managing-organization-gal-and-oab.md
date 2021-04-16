---
title: ניהול רשימת כתובות כלל ארגונית ופנקס כתובות לא מקוון
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794833"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="b682e-102">ניהול רשימת כתובות כללית (GAL) ופנקס כתובות לא מקוון (OAB) ארגוניים</span><span class="sxs-lookup"><span data-stu-id="b682e-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="b682e-103">רשימת כתובות כללית היא רשימה של אובייקטים מותאמי דואר (כל סוג של נמען שיכול לקבל דואר אלקטרוני) בארגון.</span><span class="sxs-lookup"><span data-stu-id="b682e-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="b682e-104">רשימת כתובות כללית אחת נוצרת באופן אוטומטי בכל ארגון.</span><span class="sxs-lookup"><span data-stu-id="b682e-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="b682e-105">באפשרותך ליצור רשימות כתובות כלליות נוספות כדי להפריד משתמשים לפי ארגון או מיקום, אך משתמש יחיד יכול לראות ולהשתמש ברשימת כתובות כללית אחת בלבד בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="b682e-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="b682e-106">לקוחות דואר אלקטרוני מסוימים, כגון Outlook עבור Windows, מורידים רשימת כתובות כללית לשימוש במצב לא מקוון.</span><span class="sxs-lookup"><span data-stu-id="b682e-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="b682e-107">זה נקרא פנקס כתובות לא מקוון (OAB).</span><span class="sxs-lookup"><span data-stu-id="b682e-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="b682e-108">ב-Exchange מקוון, פנקס כתובות לא מקוון מתעדכן פעם אחת בלבד כל 8 שעות, ולאחר מכן הלקוחות חייבים להוריד אותו כדי לעדכן את העותק המקומי של פנקס הכתובות הלא מקוון.</span><span class="sxs-lookup"><span data-stu-id="b682e-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="b682e-109">כל שינוי של נמען חייב להשתקף קודם ברשימת כתובות כללית כדי שיגיע אחר כך לפנקס כתובות לא מקוון.</span><span class="sxs-lookup"><span data-stu-id="b682e-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="b682e-110">להלן כמה הליכים נפוצים של רשימת כתובות כללית ופנקס כתובות לא מקוון:</span><span class="sxs-lookup"><span data-stu-id="b682e-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="b682e-111">מהרבה סיבות, ייתכן ותרצה להסתיר גורמים מסוימים מתוך רשימת כתובות כללית.</span><span class="sxs-lookup"><span data-stu-id="b682e-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="b682e-112">ראה [הסתר נמענים מרשימת כתובות](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="b682e-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="b682e-113">אם עליך להעניק לקבוצות ספציפיות של משתמשים תצוגות מותאמות אישית של רשימת הכתובות הכללית של הארגון, ראה [פריטי מדיניות של פנקס כתובות ב- Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="b682e-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="b682e-114">[צור רשימת כתובות כללית ב- Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) וכדי ללמוד כיצד לעבוד עם הרשאות רשימת כתובות כללית, ראה [רשימות כתובות ב- Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="b682e-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="b682e-115">שים לב שאם אתה יוצר רשימות כתובות כלליות חדשות, ייתכן שתרצה גם ליצור פנקס כתובות לא מקוון חדש.</span><span class="sxs-lookup"><span data-stu-id="b682e-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="b682e-116">ראה [הליכי פנקס כתובות לא מקוון](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="b682e-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
