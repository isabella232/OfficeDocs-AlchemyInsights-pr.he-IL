---
title: הוספת משתמשים חיצוניים לקבוצת תפוצה
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663514"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="406f6-102">הוספת משתמשים חיצוניים לקבוצת תפוצה</span><span class="sxs-lookup"><span data-stu-id="406f6-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="406f6-103">הוספת איש קשר חיצוני לקבוצת תפוצה (DG) היא תהליך בן שני שלבים:</span><span class="sxs-lookup"><span data-stu-id="406f6-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="406f6-104">צור איש קשר של דואר עבור המשתמש החיצוני:</span><span class="sxs-lookup"><span data-stu-id="406f6-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="406f6-105">במרכז הניהול, עבור אל הדף **Users**'  >  [אנשי קשר](https://admin.microsoft.com/adminportal/home#/Contact) של משתמשים '.</span><span class="sxs-lookup"><span data-stu-id="406f6-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="406f6-106">בחר **הוסף איש קשר**.</span><span class="sxs-lookup"><span data-stu-id="406f6-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="406f6-107">הקלד את המידע עבור איש הקשר שלך ובחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="406f6-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="406f6-108">הוסף את איש הקשר לדואר ל-DG:</span><span class="sxs-lookup"><span data-stu-id="406f6-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="406f6-109">במרכז הניהול, עבור אל הדף קבוצות **קבוצות**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="406f6-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="406f6-110">חפש את DG שאליה ברצונך להוסיף את המשתמש החיצוני ובחר אותו כדי לפתוח את תיבת הדו עריכה.</span><span class="sxs-lookup"><span data-stu-id="406f6-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="406f6-111">בכרטיסיה **חברים** , בחר **הצג הכל ונהל את החברים**.</span><span class="sxs-lookup"><span data-stu-id="406f6-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="406f6-112">בחר **הוסף חברים**.</span><span class="sxs-lookup"><span data-stu-id="406f6-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="406f6-113">בחר את איש הקשר לדואר שיצרת בשלב הקודם ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="406f6-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="406f6-114">אם לאחר ביצוע שלבים אלה, משתמשים חיצוניים אינם יכולים לשלוח הודעות דואר אלקטרוני ל-DG או לא לקבל הודעות דואר אלקטרוני ממנו, ייתכן ש-DG מסומנת רק לאפשר הודעות דואר אלקטרוני ממשתמשים פנימיים.</span><span class="sxs-lookup"><span data-stu-id="406f6-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="406f6-115">באפשרותך לבדוק תצורה זו ולפתור אותה בהתאם להוראות [כאן](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="406f6-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="406f6-116">**הערה:** הוראות אלה אינן חלות אם הסוג של הקבוצה הוא "Microsoft 365 group" במקום "הקבוצה תפוצה".</span><span class="sxs-lookup"><span data-stu-id="406f6-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="406f6-117">במקרה זה, באפשרותך להוסיף את המשתמש החיצוני ישירות לקבוצה מ-Outlook.</span><span class="sxs-lookup"><span data-stu-id="406f6-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="406f6-118">מידע מפורט בנושא Microsoft 365 קבוצות האורחים וכן הוראות להוספת אורחים חיצוניים ניתן למצוא [במאמר זה](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="406f6-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  