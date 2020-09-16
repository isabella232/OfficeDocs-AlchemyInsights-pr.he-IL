---
title: הקובץ פתוח לקריאה בלבד
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745585"
---
# <a name="file-open-read-only"></a><span data-ttu-id="bc017-102">הקובץ פתוח לקריאה בלבד</span><span class="sxs-lookup"><span data-stu-id="bc017-102">File open read-only</span></span>

<span data-ttu-id="bc017-103">ייתכן שתגלה שכאשר אתה פותח קבצים, הם נפתחים לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="bc017-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="bc017-104">במקרים מסוימים, מדובר באבטחה נוספת, למשל בעת פתיחת קבצים מהאינטרנט ובזמנים אחרים, ייתכן שהסיבה לכך היא הגדרה שניתן לשנות.</span><span class="sxs-lookup"><span data-stu-id="bc017-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="bc017-105">להלן כמה תרחישים שבהם קובץ פותח לקריאה בלבד ומספר שלבים שבאפשרותך לבצע כדי לשנות זאת.</span><span class="sxs-lookup"><span data-stu-id="bc017-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="bc017-106">**האנטי-וירוס שלי גורם להם לפתוח לקריאה בלבד**</span><span class="sxs-lookup"><span data-stu-id="bc017-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="bc017-107">תוכניות אנטי-וירוס מסוימות עשויות להגן עליך מפני קבצים שעשויים להיות לא בטוחים על-ידי פתיחתם לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="bc017-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="bc017-108">ייתכן שתצטרך לבדוק עם ספק האנטי-וירוס כדי ללמוד כיצד להתאים הגדרות אלה.</span><span class="sxs-lookup"><span data-stu-id="bc017-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="bc017-109">ל-BitDefender, לדוגמה, יש תוכן בנושא הוספת אי-הכללה של יישומים כאן: [כיצד להוסיף אי-הכללה של יישומים או תהליכים במרכז הבקרה של Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="bc017-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="bc017-110">**האם מאפייני הקובץ מוגדרים לקריאה בלבד?**</span><span class="sxs-lookup"><span data-stu-id="bc017-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="bc017-111">ניתן לבדוק את מאפייני הקובץ על-ידי לחיצה באמצעות לחצן העכבר הימני על הקובץ ובחירת מאפיינים.</span><span class="sxs-lookup"><span data-stu-id="bc017-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="bc017-112">אם התכונה ' לקריאה בלבד ' מסומנת, באפשרותך לבטל את הסימון וללחוץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="bc017-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="bc017-113">**התוכן נמצא בתצוגה מוגנת**</span><span class="sxs-lookup"><span data-stu-id="bc017-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="bc017-114">קבצים מהאינטרנט וממיקומים אחרים שעלולים להיות לא בטוחים יכולים להכיל וירוסים, תולעים או סוגים אחרים של תוכנות זדוניות שעלולות לפגוע במחשב שלך.</span><span class="sxs-lookup"><span data-stu-id="bc017-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="bc017-115">פעולה זו מתבצעת גם בדרך כלל עם קבצים מצורפים לדואר אלקטרוני או קבצים שהורדת.</span><span class="sxs-lookup"><span data-stu-id="bc017-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="bc017-116">כדי לסייע בהגנה על המחשב שלך, קבצים ממיקומים אלה שעלולים להיות לא בטוחים נפתחים בתצוגה מוגנת.</span><span class="sxs-lookup"><span data-stu-id="bc017-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="bc017-117">באמצעות תצוגה מוגנת, באפשרותך לקרוא קובץ ולראות את התוכן שלו תוך צמצום הסיכונים.</span><span class="sxs-lookup"><span data-stu-id="bc017-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="bc017-118">לקבלת מידע נוסף אודות תצוגה מוגנת וכיצד לשנות הגדרות, עיין במאמר זה: [מהי תצוגה מוגנת?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="bc017-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="bc017-119">**האם OneDrive מלא?**</span><span class="sxs-lookup"><span data-stu-id="bc017-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="bc017-120">אם הקובץ מאוחסן ב-OneDrive ושטח האחסון של OneDrive מלא, לא תוכל לשמור את המסמך עד שתהיה מתחת לשטח המוקצה.</span><span class="sxs-lookup"><span data-stu-id="bc017-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="bc017-121">באפשרותך לבדוק את השטח הפנוי שלך ב-OneDrive על-ידי לחיצה על סמל OneDrive במרכז ההודעות ובחירה באפשרות ניהול אחסון, או באפשרותך לעבור אל, להיכנס [https://onedrive.live.com](https://onedrive.live.com) ולציין את כמות השטח הנמצא בשימוש בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="bc017-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="bc017-122">**האם Office מופעל?**</span><span class="sxs-lookup"><span data-stu-id="bc017-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="bc017-123">אם Office אינו מופעל, או אם תוקפו של המנוי פג, ייתכן שאתה נמצא במצב פונקציונליות מופחתת לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="bc017-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="bc017-124">לקבלת מידע אודות אופן ההפעלה של Office, ראה: [שגיאות מוצר ללא רשיון והפעלה ב-Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="bc017-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="bc017-125">**אם כל השאר נכשל...**</span><span class="sxs-lookup"><span data-stu-id="bc017-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="bc017-126">נסה להפעיל מחדש את המחשב</span><span class="sxs-lookup"><span data-stu-id="bc017-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="bc017-127">התקנת עדכוני Office</span><span class="sxs-lookup"><span data-stu-id="bc017-127">Install Office updates</span></span>
    
- <span data-ttu-id="bc017-128">ביצוע תיקון מקוון של Office</span><span class="sxs-lookup"><span data-stu-id="bc017-128">Perform an Online repair of Office</span></span>
    

