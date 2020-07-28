---
title: האישור של Apple MDM דחיפה לא הוגדר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439383"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="bf0e0-102">האישור של Apple MDM דחיפה לא הוגדר</span><span class="sxs-lookup"><span data-stu-id="bf0e0-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="bf0e0-103">אישור Apple MDM לדחוף (הידוע גם כאישור APNS של אפל שירות הודעות) לא נקבעה עבור המנוי שלך.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="bf0e0-104">ללא אישור של אפל MDM לדחוף מוגדר, אתה לא יכול להירשם ולנהל מכשירי iOS ו-Mac OS.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="bf0e0-105">לאחר הוספת האישור ל-Intune, משתמשים יכולים להתקין את יישום הפורטל של החברה כדי לרשום את מכשירי ה-iOS שלהם.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="bf0e0-106">בחר **"אני מסכים".**</span><span class="sxs-lookup"><span data-stu-id="bf0e0-106">Select **"I agree."**</span></span> <span data-ttu-id="bf0e0-107">כדי להעניק למיקרוסופט הרשאה לשלוח נתונים ל-Apple.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="bf0e0-108">בחר באפשרות הורד את ה- **CSR שלך** לבקשת חתימת האישור הIntune הדרושה ליצירת אישור לדחיפה של Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="bf0e0-109">הקובץ משמש לבקשת אישור של יחסי אמון מפורטל האישורים של Apple Push.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="bf0e0-110">בחר באפשרות **צור אישור הדחיפה MDM שלך** כדי לעבור אל פורטל האישורים של אפל פוש.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="bf0e0-111">היכנס באמצעות מזהה Apple של החברה שלך ולאחר מכן בחר **באפשרות צור אישור**.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="bf0e0-112">בחר **באפשרות ' בחר קובץ**', דפדף אל קובץ הבקשה לחתימת האישור ולאחר מכן בחר באפשרות ' **העלאה**'.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="bf0e0-113">בדף ' אישור ', בחר באפשרות ' **הורד** ' כדי להוריד את קובץ האישור (. pem) ושמור את הקובץ באופן מקומי.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="bf0e0-114">**הערה**: האישור משויך למזהה האפל המשמש ליצירתו.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="bf0e0-115">כשיטה מיטבית, השתמש במזהה Apple של החברה עבור משימות ניהול, וודא שתיבת הדואר מנוטרת על-ידי יותר מאדם אחד או על-ידי שימוש ברשימת תפוצה.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="bf0e0-116">לעולם אל תשתמש במזהה אפל אישי.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="bf0e0-117">השתמש באותו מזהה אפל כדי לחדש את אישור אפל דחיפה כל 12 חודשים.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="bf0e0-118">הזן את מזהה Apple המשמש ליצירת אישור הדחיפה של Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="bf0e0-119">הקלט מזהה זה כתזכורת עבור המועד הדרוש לחידוש האישור.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="bf0e0-120">עבור אל קובץ האישור (. pem), בחר באפשרות **פתיחה**ולאחר מכן בחר באפשרות **העלאה**.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="bf0e0-121">עם אישור לדחוף, Intune יכול להירשם ולנהל התקני אפל.</span><span class="sxs-lookup"><span data-stu-id="bf0e0-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>