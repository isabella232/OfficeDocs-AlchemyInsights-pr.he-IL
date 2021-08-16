---
title: Intune Exchange מחבר מקומי
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013965"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange מחבר מקומי

לקבלת פרטים אודות הגדרת המחבר בין Intune Exchange המתארח באופן מקומי, עיין בתיעוד הבא:

[הגדרת המחבר המקומי Intune Exchange Intune ב- Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**שאלות נפוצות:**

ש: אני רואה שגיאה כגון "גירסת Exchange Connector אינה נתמכת" בעת ניסיון להגדיר את Exchange המחבר. מה יכול להיות הגורם?

ת: החשבון שאתה משתמש בו מורשה כראוי - חייב להיות לו רשיון Intune פעיל

ש: האם ניתן להוסיף מחברים Exchange מרובים?

ת: באפשרותך להגדיר מחבר Exchange אחד לכל דייר Intune לכל Exchange הארגון. ניתן להתקין את המחבר בשרת אחד בלבד בארגון Exchange מרובה שרתים.

כמו כן, לא ניתן להגדיר מחברים עבור Exchange באופן מקומי Exchange Online באותו דייר.

ש: האם המחבר יכול להשתמש במערך CAS כחיבור שלו Exchange?

ת: ציון מערך CAS אינו תצורה נתמכת בהגדרת המחבר. יש לציין שרת יחיד בלבד ויש לקודד אותו באופן קשיח בקובץ התצורה של המחבר, שבו ניתן למצוא

נתוני תוכנית\microsoft Intune באופן Exchange מחבר\ OnpremiseExchangeConnectorServiceConfiguration.xml

אתר את הערך הבא ```<ExchangeWebServiceURL />``` והחלף את כתובת ה- URL בשרת Exchange.

**דוגמה:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

עיין בתיעוד הבא לפתרון בעיות נוסף: פתרון בעיות במחבר [Intune Exchange המקומי](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**הפעלת רישום Verbose עבור Exchange המחבר**

1. פתח את Exchange תצורת המעקב של מחבר לעריכה.  
הקובץ ממוקם ב: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**דוגמה:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. אתר את TraceSourceLine עם המפתח הבא: OnPremisesExchangeConnectorService  
  
3. שינוי ערך הצומת SourceLevel מתוך פעילות מידע (ברירת המחדל) ל- Verbose ActivityTracing  

**דוגמה:**
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
4. הפעל מחדש את Microsoft Intune Exchange השירות  
5. סינכרון מלא בפורטל Intune עד לסיום ה- XML ולאחר מכן שנה את ה- XML בחזרה ל- "Information ActivityTracing" והפעל מחדש את Microsoft Intune Exchange השירות.  
6. מיקום יומני הרישום הוא : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`