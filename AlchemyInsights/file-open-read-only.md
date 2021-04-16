---
title: קובץ פתוח לקריאה בלבד
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813185"
---
# <a name="file-open-read-only"></a><span data-ttu-id="12788-102">קובץ פתוח לקריאה בלבד</span><span class="sxs-lookup"><span data-stu-id="12788-102">File open read-only</span></span>

<span data-ttu-id="12788-103">ייתכן שנגלה כי בעת פתיחת קבצים, הם נפתחים לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="12788-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="12788-104">במקרים מסוימים, אפשרות זו כוללת אבטחה נוספת, כגון בעת פתיחת קבצים מהאינטרנט, ובפעמים אחרות, ייתכן שההגדרה תשתנה.</span><span class="sxs-lookup"><span data-stu-id="12788-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="12788-105">להלן כמה תרחישים הראשונים לקובץ שנפתח לקריאה בלבד, וחלק מהשלבים שתוכל לבצע כדי לשנות זאת.</span><span class="sxs-lookup"><span data-stu-id="12788-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="12788-106">**האנטי-וירוס שלי גורם להם לפתוח לקריאה בלבד**</span><span class="sxs-lookup"><span data-stu-id="12788-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="12788-107">תוכניות אנטי-וירוס מסוימות עשויות להגן עליך מפני קבצים שעלולים להיות לא בטוחים על-ידי פתיחתן לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="12788-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="12788-108">ייתכן שתצטרך לבדוק עם ספק האנטי-וירוס שלך כדי ללמוד כיצד להתאים הגדרות אלה.</span><span class="sxs-lookup"><span data-stu-id="12788-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="12788-109">BitDefender, לדוגמה, כולל תוכן אודות הוספת אי-הכללות של יישומים כאן: כיצד להוסיף אי-הכללות של יישומים או תהליכים במרכז הבקרה של [Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="12788-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="12788-110">**האם מאפייני הקובץ מוגדרים לקריאה בלבד?**</span><span class="sxs-lookup"><span data-stu-id="12788-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="12788-111">באפשרותך לבדוק את מאפייני הקובץ על-ידי לחיצה באמצעות לחצן העכבר הימני על הקובץ ובחירת מאפיינים.</span><span class="sxs-lookup"><span data-stu-id="12788-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="12788-112">אם התכונה לקריאה בלבד מסומנת, באפשרותך לבטל את הסימון שלה וללחוץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="12788-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="12788-113">**התוכן נמצא בתצוגה מוגנת**</span><span class="sxs-lookup"><span data-stu-id="12788-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="12788-114">קבצים מהאינטרנט וממקומות אחרים שעלולים להיות לא בטוחים יכולים להכיל וירוסים, תולעים או סוגים אחרים של תוכנות זדוניות שעלולים להזיק למחשב שלך.</span><span class="sxs-lookup"><span data-stu-id="12788-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="12788-115">הדבר גם נפוץ עם קבצים מצורפים לדואר אלקטרוני או קבצים שהורדת.</span><span class="sxs-lookup"><span data-stu-id="12788-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="12788-116">כדי לסייע בהגנה על המחשב שלך, קבצים ממקומות שעלולים להיות לא בטוחים אלה נפתחים בתצוגה מוגנת.</span><span class="sxs-lookup"><span data-stu-id="12788-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="12788-117">באמצעות תצוגה מוגנת, באפשרותך לקרוא קובץ ולראות את התוכן שלו תוך צמצום הסיכונים.</span><span class="sxs-lookup"><span data-stu-id="12788-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="12788-118">לקבלת מידע נוסף אודות תצוגה מוגנת ואופן שינוי ההגדרות, עיין במאמר זה: [מהי תצוגה מוגנת?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="12788-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="12788-119">**האם OneDrive מלא?**</span><span class="sxs-lookup"><span data-stu-id="12788-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="12788-120">אם הקובץ מאוחסן ב- OneDrive ונפח האחסון שלך ב- OneDrive מלא, לא תוכל לשמור את המסמך עד שתמלא את השטח שהוקצה לך.</span><span class="sxs-lookup"><span data-stu-id="12788-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="12788-121">באפשרותך לבדוק את השטח הפנוי שלך ב- OneDrive על-ידי לחיצה על סמל OneDrive במרכז ההודעות ובחירה באפשרות נהל שטח אחסון, או לעבור אל , להיכנס ולציין את כמות השטח בשימוש בחלק הימני התחתון [https://onedrive.live.com](https://onedrive.live.com) של המסך.</span><span class="sxs-lookup"><span data-stu-id="12788-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="12788-122">**האם Office מופעל?**</span><span class="sxs-lookup"><span data-stu-id="12788-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="12788-123">אם Office אינו מופעל, או אם פג תוקפו של המנוי שלך, ייתכן שאתה נמצא במצב פונקציונליות מופחתת לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="12788-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="12788-124">לקבלת מידע אודות הפעלת Office, ראה: שגיאות מוצר [ללא רשיון והפעלה ב- Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="12788-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="12788-125">**אם כל השאר נכשל...**</span><span class="sxs-lookup"><span data-stu-id="12788-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="12788-126">נסה להפעיל מחדש את המחשב</span><span class="sxs-lookup"><span data-stu-id="12788-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="12788-127">התקנת עדכוני Office</span><span class="sxs-lookup"><span data-stu-id="12788-127">Install Office updates</span></span>
    
- <span data-ttu-id="12788-128">ביצוע תיקון מקוון של Office</span><span class="sxs-lookup"><span data-stu-id="12788-128">Perform an Online repair of Office</span></span>
    

