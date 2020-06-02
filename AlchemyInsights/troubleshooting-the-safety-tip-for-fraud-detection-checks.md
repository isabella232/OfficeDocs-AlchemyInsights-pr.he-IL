---
title: פתרון בעיות בעצת הבטיחות עבור בדיקות זיהוי הונאות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504984"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="a55cc-102">פתרון בעיות בעצת הבטיחות עבור בדיקות זיהוי הונאות</span><span class="sxs-lookup"><span data-stu-id="a55cc-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="a55cc-103">אם אתה מקבל עצה בטיחות שאומרת "השולח נכשל בבדיקות ההונאה שלנו וייתכן שהוא אינו מי שהם נראים", אזי השולח לא הצליח לעבור בדיקות אימות DKIM או SPF.</span><span class="sxs-lookup"><span data-stu-id="a55cc-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="a55cc-104">השיטה הטובה ביותר לפתרון זה היא שהשולח יאשר את עצמו.</span><span class="sxs-lookup"><span data-stu-id="a55cc-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="a55cc-105">אם השולח שולח בשמך, עליך לאשר אותם על-ידי הוספת כתובת ה-IP של השולח לרשומת SPF.</span><span class="sxs-lookup"><span data-stu-id="a55cc-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="a55cc-106">ראה [פתרון בעיות בעצת הבטיחות האדומה (החשודה) לקבלת מידע נוסף על בדיקות זיהוי הונאות](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="a55cc-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="a55cc-107">להלן כמה קישורים אחרים שיכולים לעזור:</span><span class="sxs-lookup"><span data-stu-id="a55cc-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="a55cc-108">כיצד משתמש Microsoft במסגרת מדיניות השולח (SPF) כדי למנוע זיופים</span><span class="sxs-lookup"><span data-stu-id="a55cc-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="a55cc-109">הגדר SPF כדי לסייע במניעת זיופים</span><span class="sxs-lookup"><span data-stu-id="a55cc-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
