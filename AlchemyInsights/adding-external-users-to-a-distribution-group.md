---
title: הוספת משתמשים חיצוניים לקבוצת תפוצה
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910933"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="40d89-102">הוספת משתמשים חיצוניים לקבוצת תפוצה</span><span class="sxs-lookup"><span data-stu-id="40d89-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="40d89-103">הוספת איש קשר חיצוני לקבוצת תפוצה (DG) היא תהליך בן שני שלבים:</span><span class="sxs-lookup"><span data-stu-id="40d89-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="40d89-104">צור איש קשר של דואר עבור המשתמש החיצוני:</span><span class="sxs-lookup"><span data-stu-id="40d89-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="40d89-105">במרכז הניהול, עבור אל דף **Users** > [אנשי הקשר](https://admin.microsoft.com/adminportal/home#/Contact) של Users.</span><span class="sxs-lookup"><span data-stu-id="40d89-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="40d89-106">בחר **בהוסף איש קשר**.</span><span class="sxs-lookup"><span data-stu-id="40d89-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="40d89-107">הקלד את המידע עבור איש הקשר שלך ובחר **ב'הוספה**.</span><span class="sxs-lookup"><span data-stu-id="40d89-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="40d89-108">הוסף את איש הקשר לדואר ל-DG שלך:</span><span class="sxs-lookup"><span data-stu-id="40d89-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="40d89-109">במרכז הניהול, עבור לדף קבוצות **קבוצות** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="40d89-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="40d89-110">חפש את ה-DG שאליה ברצונך להוסיף את המשתמש החיצוני ובחר בו כדי לפתוח את תיבת הדו של העריכה.</span><span class="sxs-lookup"><span data-stu-id="40d89-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="40d89-111">בכרטיסיה **חברים** , בחר **באפשרות הצג הכל ונהל את החברים**.</span><span class="sxs-lookup"><span data-stu-id="40d89-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="40d89-112">בחר באפשרות ' **הוסף חברים**'.</span><span class="sxs-lookup"><span data-stu-id="40d89-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="40d89-113">בחר את איש הקשר של הדואר שיצרת בשלב הקודם ולאחר מכן בחר **בשמור**.</span><span class="sxs-lookup"><span data-stu-id="40d89-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="40d89-114">אם לאחר ביצוע שלבים אלה המשתמשים החיצוניים שלך לא יכולים לשלוח מיילים ל-DG או לא לקבל מיילים ממנו, זה יכול להיות כי DG מסומנת רק לאפשר מיילים ממשתמשים פנימיים.</span><span class="sxs-lookup"><span data-stu-id="40d89-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="40d89-115">באפשרותך לבדוק תצורה זו ולתקן אותה לאחר ההנחיות [כאן](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="40d89-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="40d89-116">**הערה:** הוראות אלה אינן חלות אם סוג הקבוצה שלך הוא "Microsoft 365 group" במקום "קבוצת תפוצה".</span><span class="sxs-lookup"><span data-stu-id="40d89-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="40d89-117">אם זהו המצב, באפשרותך להוסיף את המשתמש החיצוני ישירות לקבוצה מ-Outlook.</span><span class="sxs-lookup"><span data-stu-id="40d89-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="40d89-118">מידע מפורט על מיקרוסופט 365 קבוצות אורחים, כמו גם הוראות להוספת אורחים חיצוניים ניתן למצוא [במאמר זה](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="40d89-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  