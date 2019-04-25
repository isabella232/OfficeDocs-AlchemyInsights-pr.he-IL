---
title: פתרון בעיות העצה בטיחות לאיתור הונאה בודק
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391210"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ad2c4-102">פתרון בעיות העצה בטיחות לאיתור הונאה בודק</span><span class="sxs-lookup"><span data-stu-id="ad2c4-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="ad2c4-103">אם אתה מקבל עצה בטיחות אשר אומר "השולח נכשל שלנו בדיקות זיהוי הונאה וייתכן שלא מי הם מופיעים" ולאחר מכן השולח נכשל לעבור בדיקות אימות DKIM או SPF.</span><span class="sxs-lookup"><span data-stu-id="ad2c4-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ad2c4-104">השיטה הטובה ביותר כדי לפתור בעיה זו היא עבור השולח לאשר את עצמם.</span><span class="sxs-lookup"><span data-stu-id="ad2c4-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ad2c4-105">אם השולח שולח בשמך, עליך לאשר אותם על-ידי הוספת כתובת ה-IP של השולח רשומת SPF שלך.</span><span class="sxs-lookup"><span data-stu-id="ad2c4-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ad2c4-106">לקבלת מידע נוסף, ראה [פתרון בעיות העצה בטיחות (חשוד) אדום לאיתור הונאה בודק](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="ad2c4-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="ad2c4-107">להלן מספר קישורים אחרים שיכולים לסייע:</span><span class="sxs-lookup"><span data-stu-id="ad2c4-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ad2c4-108">כיצד Office 365 משתמש מסגרת המדיניות של השולח (SPF) כדי למנוע זיוף</span><span class="sxs-lookup"><span data-stu-id="ad2c4-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="ad2c4-109">הגדרת SPF ב- Office 365 למניעת התחזות</span><span class="sxs-lookup"><span data-stu-id="ad2c4-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

