---
title: מחבר מקומי של Exchange של כוונון האתר
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807648"
---
# <a name="intune-exchange-on-premise-connector"></a>מחבר מקומי של Exchange של כוונון האתר

לקבלת פרטים על הגדרת המחבר בין המנגינה לבין Exchange המתארח באופן מקומי, עיין בתיעוד הבא:

[הגדרת מחבר Exchange המקומי ב-Microsoft intune בתכלת של Microsoft](https://docs.microsoft.com/intune/exchange-connector-install)

**שאלות נפוצות**

ש: אני רואה שגיאה כגון "גירסת מחבר Exchange אינה נתמכת" בעת ניסיון להגדיר את מחבר Exchange. מה עשויה להיות הסיבה?

ת: החשבון שבו אתה משתמש מורשה כראוי-עליו לכלול רשיון של כוונון פעיל

ש: האם ניתן לכלול מחברי Exchange מרובים?

א: באפשרותך להגדיר רק מחבר Exchange אחד לכל ארגון של Exchange לכל אחד מהדיירים. ניתן להתקין את המחבר רק בשרת אחד בארגון exchange בשרת רב-ממדי.

כמו כן, לא ניתן להגדיר מחברים שתצורתם נקבעה הן עבור Exchange Online והן של Exchange Online המוגדרות באותו דייר.

ש: האם המחבר יכול להשתמש במערך CAS כחיבור שלו ל-Exchange?

ת: ציון מערך CAS אינו תצורה נתמכת בהגדרת המחבר. יש לציין רק שרת אחד ויש לקשיח בקובץ תצורת המחבר שניתן למצוא ב-

תוכנית data\microsoft\microsoft התכוונת למחבר Exchange המקומי \ OnpremiseExchangeConnectorServiceConfiguration.xml

אתר את הערך הבא ```<ExchangeWebServiceURL />``` והחלף את כתובת ה-URL בשרת exchange.

**דוגמה**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

עיין בתיעוד הבא לאיתור בעיות נוספות: [פתרון בעיות במחבר Exchange המקומי](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**הפעלת רישום Verbose עבור מחבר Exchange**

1. פתח את קובץ התצורה של עקיבה אחר מחבר Exchange לעריכה.  
הקובץ ממוקם בכתובת: Connector\TracingConfiguration.xml%ProgramData%\Microsoft\Windows של Exchange  

**דוגמה**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. אתר את TraceSourceLine עם המפתח הבא: OnPremisesExchangeConnectorService  
  
3. שינוי ערך הצומת של SourceLevel ממידע ActivityTracing (ברירת המחדל) לActivityTracing Verbose  

**דוגמה**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. הפעל מחדש את שירות החליפין של Microsoft intune  
5. סינכרון מלא בפורטל ' כוונון ' עד שהוא מסיים ולאחר מכן שנה את ה-XML חזרה ל-"Information ActivityTracing" והפעל מחדש את שירות החליפין של Microsoft intune.  
6. מיקום יומני הרישום הוא: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`