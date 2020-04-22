---
title: שימוש בכלי הפריסה של Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726249"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="3c0f2-102">שימוש בכלי הפריסה של Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="3c0f2-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="3c0f2-103">השתמש בכלי הפריסה של Office (ODT) כדי לפרוס גירסאות office 365 של Office.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="3c0f2-104">כלי הפריסה של Office (setup. exe) מופעל מתוך שורת הפקודה ומשתמש בקובץ XML של תצורה כדי לקבוע אילו הגדרות יחולו בעת פריסת Office.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="3c0f2-105">הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office [ממרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="3c0f2-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="3c0f2-106">השתמש [בכלי התאמה אישית של Office (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה שלך וליצור את קובץ ה-XML של התצורה.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="3c0f2-107">יצא את קובץ התצורה ומלא אותו באופן מקומי באותה תיקייה שבה נמצאת ההתקנה. exe.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="3c0f2-108">**הערה:** בעיות התקנה של Office מתרחשות בדרך כלל עקב קבצי תצורה שאינם מאותחלים או מעוצבים.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="3c0f2-109">כדי להימנע מבעיות כאלה, מומלץ להשתמש בכלי ההתאמה האישית של Office כדי ליצור את קובץ התצורה.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="3c0f2-110">באפשרותך גם לייבא קבצי תצורה קיימים לכלי ההתאמה האישית של Office.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="3c0f2-111">משורת פקודה עם הרשאות מלאות, עבור למיקום שבו setup. exe שוכן והפעל את כלי הפריסה של Office במצב הורדה וציין את קובץ התצורה ששמרת זה עתה.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="3c0f2-112">בדוגמה זו, קובץ התצורה נקרא תצורה. xml:</span><span class="sxs-lookup"><span data-stu-id="3c0f2-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="3c0f2-113">הפעל את כלי הפריסה של Office במצב קביעת תצורה וציין את קובץ התצורה.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="3c0f2-114">**הערה:** עליך להפעיל שלב זה ממחשב הלקוח שבו ברצונך להתקין את Office ועליך להיות בעל הרשאות מנהל מקומיות במחשב זה.</span><span class="sxs-lookup"><span data-stu-id="3c0f2-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="3c0f2-115">כדי ללמוד עוד אודות השימוש בכלי פריסת Office עבור יישומי Microsoft 365 עבור תרחישי פריסה ארגוניים, ראה [מבט כולל על כלי הפריסה של office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="3c0f2-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="3c0f2-116">לקבלת פרטים נוספים על אופן השימוש בכלי ההתאמה האישית של Office, ראה [מבט כולל על כלי ההתאמה האישית של office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="3c0f2-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
