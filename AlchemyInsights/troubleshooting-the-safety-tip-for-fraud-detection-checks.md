---
title: פתרון בעיות של תיאור הבטיחות עבור בדיקת זיהוי הונאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834732"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="d2dc9-102">פתרון בעיות של תיאור הבטיחות עבור בדיקת זיהוי הונאות</span><span class="sxs-lookup"><span data-stu-id="d2dc9-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="d2dc9-103">אם אתה מקבל עצה בטיחותית שאומרת "השולח נכשל בזיהוי ההונאה שלנו ו ייתכן שהוא אינו מי שהוא נראה", השולח לא הצליח להעביר בדיקת אימות DKIM או SPF.</span><span class="sxs-lookup"><span data-stu-id="d2dc9-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="d2dc9-104">השיטה הטובה ביותר לפתור בעיה זו היא שהשולח יאשר את עצמו.</span><span class="sxs-lookup"><span data-stu-id="d2dc9-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="d2dc9-105">אם השולח שולח בשמך, עליך לאשר אותו על-ידי הוספת כתובת ה- IP של השולח אל רשומת ה- SPF שלך.</span><span class="sxs-lookup"><span data-stu-id="d2dc9-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="d2dc9-106">לקבלת [מידע נוסף, ראה פתרון בעיות של עצה הבטיחות האדומה (החשודה)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) לאיתור הונאות.</span><span class="sxs-lookup"><span data-stu-id="d2dc9-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="d2dc9-107">להלן כמה קישורים אחרים ה יכולים לעזור:</span><span class="sxs-lookup"><span data-stu-id="d2dc9-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="d2dc9-108">כיצד Microsoft משתמשת במסגרת מדיניות השולח (SPF) כדי למנוע תיפוף</span><span class="sxs-lookup"><span data-stu-id="d2dc9-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="d2dc9-109">הגדרת SPF כדי לסייע במניעת תיפוך</span><span class="sxs-lookup"><span data-stu-id="d2dc9-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
