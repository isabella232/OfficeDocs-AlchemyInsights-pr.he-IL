---
title: פרישת שירותים של Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698683"
---
# <a name="access-services-retirement"></a>פרישת שירותים של Access

כפי שהכרזתי במקור ב-MC97576, במרץ 2017, והמשכנו לקיים תקשורת במהלך השנה החולפת של Access שירותי הגישה מפורשים. השלב הבא בתהליך זה יהיה הסרת מסדי נתונים של Access המשתמשים ברשימות SharePoint כאחסון הנתונים המשמש כבסיס.

**כיצד זה משפיע עלי?**

החל מיוני 2019, אנו נעצור את היצירה של מסדי נתונים חדשים של Access ב-SharePoint Online ונכבה את השירות ואת כל היישומים הנותרים על-ידי אפריל 2020.

**מה עליי לעשות כדי להתכונן לשינוי זה?**

אנו ממליצים לך ליצור תוכנית מעבר עבור מסדי הנתונים באינטרנט של Access בארגון שלך. מנהלי מערכת יכולים להשתמש [בסורק היישומים של SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) כדי לקבל מלאי של יישומי Access שבהם משתמש האתרים.

קיימות כמה דרכים להעברת נתונים של מסדי נתונים באינטרנט של Access:

- ייבוא למסד נתונים מקומי של Access (. ACCDB) או לקובץ Excel.
- כמו כן, אנו ממליצים לחקור את Microsoft PowerApps כפלטפורמה חלופית כדי ליצור פתרונות עסקיים ללא קוד עבור מכשירים באינטרנט ובמכשירים ניידים.