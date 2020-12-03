---
title: מחיקת דייר
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564620"
---
# <a name="delete-tenant"></a><span data-ttu-id="a65e8-102">מחיקת דייר</span><span class="sxs-lookup"><span data-stu-id="a65e8-102">Delete tenant</span></span>

<span data-ttu-id="a65e8-103">כדי למחוק מודעה של תכלת, ודא כי:</span><span class="sxs-lookup"><span data-stu-id="a65e8-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="a65e8-104">אתה מנהל מערכת כללי במדריך הכתובות.</span><span class="sxs-lookup"><span data-stu-id="a65e8-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="a65e8-105">לא נכנסת באמצעות חשבון בעל מדריך הכתובות המוגדר כברירת מחדל, כגון contoso.onmicrosoft.com בחשבון החתום, כגון admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="a65e8-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="a65e8-106">הסר את כל היישומים הפעילים במדריך הכתובות לפני המחיקה.</span><span class="sxs-lookup"><span data-stu-id="a65e8-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="a65e8-107">כדי להסיר יישומים פעילים, נווט אל רישומי היישומים והסר את היישומים הקיימים.</span><span class="sxs-lookup"><span data-stu-id="a65e8-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="a65e8-108">אין מנויים פעילים עבור שירותים מקוונים של Microsoft, כגון Microsoft התכלת, Office 365 או תכלת AD Premium המשויכים למדריך הכתובות.</span><span class="sxs-lookup"><span data-stu-id="a65e8-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="a65e8-109">העבר את המנויים שלך או ביטול מזורז של מנויים פעילים באמצעות תמיכה וחיובים של תכלת.</span><span class="sxs-lookup"><span data-stu-id="a65e8-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="a65e8-110">קבל מידע נוסף על ביטול מנויים של Office 365 ו-תכלת.</span><span class="sxs-lookup"><span data-stu-id="a65e8-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="a65e8-111">לקבלת הנחיות לגבי שיוך או הוספה של מנוי קיים לדייר, ראה [שיוך או הוספה של מנוי תכלת לדייר הודעות תכלת](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="a65e8-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="a65e8-112">אין רשיון פעיל.</span><span class="sxs-lookup"><span data-stu-id="a65e8-112">There are no Active license.</span></span> <span data-ttu-id="a65e8-113">כדי להסיר רשיונות, ראה [כיצד להסיר מנוי כדי להסיר את הרשיון](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="a65e8-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="a65e8-114">אין משתמשים פעילים נוספים במדריך הכתובות מלבד עצמך כמנהל המערכת הכללי כאשר אתה מנסה למחוק את ' תכלת AD '.</span><span class="sxs-lookup"><span data-stu-id="a65e8-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="a65e8-115">הסר משתמשים פעילים אחרים, וכל יחסי התלות של שם תחום מותאם אישית בדייר יצטרכו גם הם להסרה, כגון משתמשים שנוצרו באמצעות admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="a65e8-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="a65e8-116">לקבלת שלבים נוספים לפירוט:</span><span class="sxs-lookup"><span data-stu-id="a65e8-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="a65e8-117">מחק את ' תכלת Active Directory ' או ' מנוי ', ראה [מחיקת מדריך כתובות של Active directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="a65e8-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="a65e8-118">הסרת יישומים במדריך הכתובות, ראה [הסרת יישומים](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="a65e8-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
