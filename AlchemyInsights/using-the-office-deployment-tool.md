---
title: שימוש בכלי הפריסה של Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292559"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="7b041-102">שימוש בכלי הפריסה של Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="7b041-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="7b041-p101">שימוש בכלי הפריסה של Office (ODT) כדי לפרוס גירסאות Office 365 של Office. כלי הפריסה של Office (setup.exe) פועלת מתוך שורת הפקודה ומשתמש קובץ XML תצורה כדי לקבוע אילו הגדרות כדי להחיל בעת פריסת Office.</span><span class="sxs-lookup"><span data-stu-id="7b041-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="7b041-105">הורד את הגירסה העדכנית ביותר של כלי הפריסה של Office דרך [מרכז ההורדות של Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="7b041-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="7b041-p102">השתמש [בכלי ההתאמה האישית של Office (OCT)](https://config.office.com) כדי לבחור את העדפות הפריסה שלך וליצור קובץ ה-XML של התצורה. ייצוא קובץ התצורה והעבר אותו באופן מקומי באותה תיקיה בה שוכן setup.exe.</span><span class="sxs-lookup"><span data-stu-id="7b041-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="7b041-p103">**הערה:** התקנת office בעיות בדרך כלל מתרחשים יעד שתצורתו אינה מוגדרת כראוי או קבצי תצורה של malformatted. כדי להימנע מבעיות מסוג זה, אנו ממליצים להשתמש בכלי ההתאמה האישית של Office כדי ליצור את קובץ התצורה. באפשרותך גם לייבא קבצי תצורה קיימים לתוך כלי ההתאמה האישית של Office.</span><span class="sxs-lookup"><span data-stu-id="7b041-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="7b041-p104">משורת פקודה עם הרשאות מלאות, לעבור אל המיקום בו שוכן setup.exe להפעיל את כלי הפריסה של Office במצב ההורדה וציין את קובץ התצורה שזה עתה שמרת. בדוגמה זו, קובץ התצורה בשם Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="7b041-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="7b041-113">הפעל את כלי הפריסה של Office בתצורה של מצב וציין את קובץ התצורה.</span><span class="sxs-lookup"><span data-stu-id="7b041-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="7b041-114">**הערה:** עליך להפעיל את שלב זה מתוך מחשב הלקוח שבו ברצונך להתקין את Office ודרושות לך הרשאות מנהל מערכת מקומי במחשב זה.</span><span class="sxs-lookup"><span data-stu-id="7b041-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="7b041-p105">כדי ללמוד עוד אודות שימוש בכלי הפריסה של Office עבור Office 365 ProPlus תרחישי הפריסה, ראה [מבט כולל על כלי הפריסה של Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). לקבלת פרטים נוספים על אופן השימוש בכלי ההתאמה האישית של Office, ראה [מבט כולל על כלי ההתאמה האישית של Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="7b041-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

