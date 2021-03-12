---
title: שליחת הודעת דואר אלקטרוני על-ידי מתן מזהה הודעת רשת
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745521"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="e6489-102">שליחת הודעת דואר אלקטרוני על-ידי מתן מזהה הודעת רשת</span><span class="sxs-lookup"><span data-stu-id="e6489-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="e6489-103">בנשלף של **השליחה החדשה** , בחר **דואר אלקטרוני** **ומזהה הודעת רשת**.</span><span class="sxs-lookup"><span data-stu-id="e6489-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="e6489-104">בצע שלבים אלה כדי לאתר את מזהה ההודעה עבור הודעת דואר אלקטרוני ב-Outlook:</span><span class="sxs-lookup"><span data-stu-id="e6489-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="e6489-105">לחץ פעמיים על הודעת הדואר האלקטרוני כדי לפתוח אותה.</span><span class="sxs-lookup"><span data-stu-id="e6489-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="e6489-106">בחר   >  **מאפייני** קובץ.</span><span class="sxs-lookup"><span data-stu-id="e6489-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="e6489-107">פתח את פנקס הרשימות או מסמך Word ריק, ולאחר מכן העתק והדבק את התוכן שנמצא בתיבה **כותרות אינטרנט** למסמך הפתוח לקבלת ניראות טובה יותר.</span><span class="sxs-lookup"><span data-stu-id="e6489-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="e6489-108">אתר את ה **-X-MS-Exchange-ארגון-השדה ' מזהה הודעות רשת** '.</span><span class="sxs-lookup"><span data-stu-id="e6489-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="e6489-109">הערך אחרי **:** הוא המזהה הדרוש לך עבור השליחה.</span><span class="sxs-lookup"><span data-stu-id="e6489-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="e6489-110">תחת **נמענים**, אם הודעת הדואר האלקטרוני נחתה בתיקיה ' דואר זבל ' עבור כל הנמענים של הודעת דואר אלקטרוני זו, בחר **באפשרות בחר הכל**.</span><span class="sxs-lookup"><span data-stu-id="e6489-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="e6489-111">אם לא, בחר רק את המשתמש שדיווח על הבעיה.</span><span class="sxs-lookup"><span data-stu-id="e6489-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="e6489-112">תחת **סיבה לשליחה**, אם בחרת באפשרות **להיות חסום**, ציין אם ההודעה הייתה אמורה להיות חסומה כהודעת **זבל**, **דיוג** או **תוכנות זדוניות** ולאחר מכן בחר **שלח**.</span><span class="sxs-lookup"><span data-stu-id="e6489-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="e6489-113">לקבלת מידע נוסף, ראה [כיצד לשלוח הודעות זבל חשודות, פיש, כתובות url וקבצים ל-Microsoft לסריקה](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="e6489-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
