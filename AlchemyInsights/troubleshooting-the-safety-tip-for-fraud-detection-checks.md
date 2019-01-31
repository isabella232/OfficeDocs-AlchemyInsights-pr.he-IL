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
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658116"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="f1183-102">פתרון בעיות העצה בטיחות לאיתור הונאה בודק</span><span class="sxs-lookup"><span data-stu-id="f1183-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="f1183-p101">אם אתה מקבל עצה בטיחות אשר אומר "השולח נכשל שלנו בדיקות זיהוי הונאה וייתכן שלא מי הם מופיעים" ולאחר מכן השולח נכשל לעבור בדיקות אימות DKIM או SPF. השיטה הטובה ביותר כדי לפתור בעיה זו היא עבור השולח לאשר את עצמם. אם השולח שולח בשמך, עליך לאשר אותם על-ידי הוספת כתובת ה-IP של השולח רשומת SPF שלך.</span><span class="sxs-lookup"><span data-stu-id="f1183-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="f1183-106">לקבלת מידע נוסף, ראה [פתרון בעיות העצה בטיחות (חשוד) אדום לאיתור הונאה בודק](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="f1183-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="f1183-107">להלן מספר קישורים אחרים שיכולים לסייע:</span><span class="sxs-lookup"><span data-stu-id="f1183-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="f1183-108">כיצד Office 365 משתמש מסגרת המדיניות של השולח (SPF) כדי למנוע זיוף</span><span class="sxs-lookup"><span data-stu-id="f1183-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="f1183-109">הגדרת SPF ב- Office 365 למניעת התחזות</span><span class="sxs-lookup"><span data-stu-id="f1183-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

