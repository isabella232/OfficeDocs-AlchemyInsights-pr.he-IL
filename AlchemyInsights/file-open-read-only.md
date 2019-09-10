---
title: פתיחת קובץ לקריאה בלבד
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822235"
---
# <a name="file-open-read-only"></a><span data-ttu-id="d4fe7-102">פתיחת קובץ לקריאה בלבד</span><span class="sxs-lookup"><span data-stu-id="d4fe7-102">File open read-only</span></span>

<span data-ttu-id="d4fe7-103">ייתכן שתגלה שבעת פתיחת קבצים, הם נפתחים לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="d4fe7-104">במקרים מסוימים, הדבר מיועד לאבטחה נוספת, כגון בעת פתיחת קבצים מהאינטרנט ופעמים אחרות, ייתכן שהסיבה לכך היא הגדרה שניתן לשנותה.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="d4fe7-105">להלן מספר תרחישים שבהם קובץ פותח לקריאה בלבד וחלק מהשלבים שבאפשרותך לבצע כדי לשנות זאת.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="d4fe7-106">**האנטי-וירוס שלי גורם להם להיפתח לקריאה בלבד**</span><span class="sxs-lookup"><span data-stu-id="d4fe7-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="d4fe7-107">תוכניות אנטי-וירוס מסוימות עשויות להגן עליך מפני קבצים שעלולים להיות לא בטוחים על-ידי פתיחתם לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="d4fe7-108">ייתכן שיהיה עליך לבדוק עם ספק האנטי-וירוס שלך כדי ללמוד כיצד לכוונן הגדרות אלה.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="d4fe7-109">BitDefender, למשל, יש תוכן על הוספת החריגים יישומים כאן: [כיצד להוסיף יישום או תהליך החריגים במרכז הבקרה של Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="d4fe7-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="d4fe7-110">**האם מאפייני הקובץ מוגדרים לקריאה בלבד?**</span><span class="sxs-lookup"><span data-stu-id="d4fe7-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="d4fe7-111">באפשרותך לבדוק את מאפייני הקובץ על-ידי לחיצה ימנית על הקובץ ובחירה באפשרות מאפיינים.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="d4fe7-112">אם התכונה ' לקריאה בלבד ' מסומנת, ניתן לבטל את הסימון וללחוץ על ' אישור '.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="d4fe7-113">**התוכן נמצא בתצוגה מוגנת**</span><span class="sxs-lookup"><span data-stu-id="d4fe7-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="d4fe7-114">קבצים מהאינטרנט וממיקומים אחרים שעלולים להיות לא בטוחים יכולים להכיל וירוסים, תולעים או סוגים אחרים של תוכנות זדוניות שעלולות להזיק למחשב שלך.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="d4fe7-115">זה גם בדרך כלל המקרה עם קבצים מצורפים דוא ל או קבצים שהורדת.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="d4fe7-116">כדי לסייע בהגנה על המחשב, קבצים ממיקומים שעלולים להיות לא בטוחים נפתחים בתצוגה מוגנת.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="d4fe7-117">באמצעות ' תצוגה מוגנת ', באפשרותך לקרוא קובץ ולראות את תוכנו תוך כדי הפחתת הסיכונים.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="d4fe7-118">לקבלת מידע נוסף אודות תצוגה מוגנת וכיצד לשנות הגדרות, ראה מאמר זה: [מהי תצוגה מוגנת?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="d4fe7-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="d4fe7-119">**? כונן אחד מלא**</span><span class="sxs-lookup"><span data-stu-id="d4fe7-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="d4fe7-120">אם הקובץ מאוחסן ב-OneDrive ושטח האחסון של OneDrive מלא, לא תוכל לשמור את המסמך עד שתהיה תחת השטח שהוקצה לך.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="d4fe7-121">באפשרותך לבדוק את השטח הפנוי שלך ב-OneDrive על-ידי לחיצה על הסמל OneDrive במרכז ההודעות ובחירה באפשרות ניהול אחסון, או שבאפשרותך לעבור אל [http://onedrive.live.com](http://onedrive.live.com), להיכנס ולשים לב לכמות השטח המשמש בחלק השמאלי התחתון של המסך.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="d4fe7-122">**האם Office מופעל?**</span><span class="sxs-lookup"><span data-stu-id="d4fe7-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="d4fe7-123">אם Office אינו מופעל, או אם פג תוקפו של המנוי שלך, תוכל להיות במצב פונקציונליות מופחתת לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="d4fe7-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="d4fe7-124">לקבלת מידע אודות אופן ההפעלה של Office, ראה: [שגיאות מוצר ללא רשיון והפעלה ב-Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="d4fe7-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="d4fe7-125">**אם כל השאר ייכשל...**</span><span class="sxs-lookup"><span data-stu-id="d4fe7-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="d4fe7-126">נסה להפעיל מחדש את המחשב</span><span class="sxs-lookup"><span data-stu-id="d4fe7-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="d4fe7-127">התקנת עדכוני Office</span><span class="sxs-lookup"><span data-stu-id="d4fe7-127">Install Office updates</span></span>
    
- <span data-ttu-id="d4fe7-128">בצע תיקון מקוון של Office</span><span class="sxs-lookup"><span data-stu-id="d4fe7-128">Perform an Online repair of Office</span></span>
    

