---
title: בעיה באיפוס סיסמה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694376"
---
# <a name="problems-resetting-password"></a>בעיות באיפוס סיסמה

להלן כמה מהבעיות שאתה עשוי לעמוד בהן בעת איפוס סיסמה ופתרונות אפשריים:

**אני נתקל בבעיה עם איפוס סיסמה שאינו מכוסה בקטגוריות האחרות**

- ודא שאתה מורשה לאפס סיסמאות. רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים. מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.
- ודא שהבנת את דרישות הרישוי:
    - דרוש לך רשיון אחד לפחות שהוקצה בארגון שלך
        - משתמשים בענן בלבד-כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic
        - משתמשים בענן ו/או מקומיים-תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)
        - לקבלת מידע נוסף אודות דרישות הרישוי, ראה [דרישות רישוי מאמר עבור איפוס סיסמה בשירות עצמי של תכלת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**אני נתקל בבעיות בבדיקת מדיניות איפוס הסיסמה שהגדרתי**

- מדיניות שהוחלו לאחרונה עשויה להימשך כמה דקות כדי לשכפל את כל מרכזי הנתונים ואת נקודות הקצה. מרחק פיסי ממרכז הנתונים ישפיע גם על החלת השינויים במהירות.
- בדיקה עם משתמש קצה, לא מנהל מערכת ופיילוט עם קבוצת משתמשים קטנה. פריטי המדיניות המוגדרים בפורטל ' תכלת ' חלים רק על משתמשי קצה, לא על מנהלי מערכת. Microsoft אוכפת מדיניות ברירת מחדל של איפוס סיסמה בשני שערים עבור כל תפקיד מנהל מערכת של תכלת (לדוגמה: מנהל מערכת כללי, מנהל מוקד התמיכה, מנהל הסיסמאות וכדומה)
    - קבל [מידע נוסף אודות פריטי מדיניות עבור מנהלי מערכת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**ברצוני לפרוס איפוס סיסמה, אך איני מעוניין לגרום למשתמשים שלי לרשום מידע אבטחה נוסף**

אכלוס מראש של נתונים עבור המשתמשים שלך כדי שלא יצטרכו! -כמנהל מערכת, באפשרותך להגדיר מאפייני טלפון ודואר אלקטרוני עבור המשתמשים שלך לפני שתפעיל את איפוס הסיסמה לארגון שלך. באפשרותך לעשות זאת באמצעות התחברות ב-API, PowerShell או תכלת לספירה. מידע נוסף כאן:
- [פריסת איפוס סיסמה מבלי לחייב משתמשים לרשום](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [אילו נתונים משמשים לאיפוס סיסמה](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**לחצן ' איפוס סיסמה ' מופיע באפור**

אין לך הרשאה לאפס את הסיסמאות של משתמש זה. רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים. מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.

**איני רואה את להב איפוס הסיסמה**

אין לך הרשאה לאפס סיסמאות. רק כללי, סיסמה ומנהלי מערכת יכולים לאפס סיסמאות משתמשים. מנהלי מערכת כלליים יכולים גם לאפס סיסמאות אחרות של מנהל מורשה.

**איני רואה את להב השילוב המקומי באיפוס סיסמה**

- להב השילוב המקומי מופיע רק בסביבות היברידיות-כלומר, אתה משתמש ב-writeback password כדי לטפל בסיסמאות של משתמש מקומי.
- אינך רואה את הלהב הזה אם:
    - אינך משתמש ב-password writeback
    - קיימת בעיה בהתקנה/בקישוריות של writeback סיסמה
    - קיימת בעיה בהתקנה/בקישוריות של התחברות של תכלת לספירה
    - לקבלת שלבים נוספים לפתרון בעיות עבור בעיות בwriteback סיסמאות, עיין בסעיף [פתרון בעיות בסיסמאות writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**איני יודע כיצד לאפס סיסמת משתמש**

1. היכנס לפורטל ' תכלת ' כמנהל מתאים.
1. עבור אל הלהב משתמשים וקבוצות, בחר **את כל המשתמשים**.
1. בחר משתמש מהרשימה.
1. עבור המשתמש שנבחר, בחר **מבט כולל** ולאחר מכן, בסרגל הפקודות, לחץ על **איפוס סיסמה**.
1. בצע את ההוראות המופיעות על המסך.
    - רק איפוסים שבוצעו באמצעות הסיסמה ' תמיכה בפורטל של writeback '.

**אני מאפס סיסמה של משתמש מקומי מפורטל הניהול של Office 365 או מהיישום Office 365 למכשירים ניידים, אך המשתמש עדיין אינו מצליח להיכנס**

Writeback סיסמה אינו נתמך בפורטל זה. איפוס סיסמת המשתמש שוב בפורטל התכלת-portal.azure.com

