---
title: הסרת נתונים ומחיקת מכשירים מ- Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416314"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>הסרת נתונים ומחיקת מכשירים מ- Intune

ניתן להשתמש בפעולות מרוחקות של 'הוצאת מכשיר משימוש' ו'מחיקת מכשיר' כדי להסיר נתוני חברה שמונעלים על-ידי Intune או כדי לבצע איפוס יצרן ולהחזיר את המכשיר להגדרות ברירת המחדל שלו.

1. היכנס לניהול המכשירים של Microsoft 365 ועבור אל **מכשירים** > **כל המכשירים**.
2. בחר את ההתקן שברצונך למחוק.
3. בחר את הסוג של המחיקה מרחוק שברצונך לבצע. הפעולה 'הוצא משימוש' מוחקת מידע ארגוני בלבד, בשעה שמחיקה מלאה משחזרת את המכשיר להגדרות היצרן שלו.
4. בחר **כן** כדי לאשר. עד לסיום המחיקה, מצב הפעולה של המכשיר יופיע ג *הוצאה משימוש ממתינה*.
    לאחר השלמת הפעולה, לא תראה עוד את המכשיר הנייד ברשימת המכשירים המנוהלים.

> [!NOTE]
> לא ניתן להסיר נתוני חברה ממכשירים שהצטרפו ל- Azure AD. 

לקבלת פרטים מלאים של השפעת פעולות 'הוצאה משימוש' ו'מחיקה', כולל מה נשמר ומה נמחק, ראה את המסמכים הבאים:

- [הסרת מכשירים על-ידי מחיקה, הוצאה משימוש או ביטול רישום של המכשיר](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [כיצד למחוק נתונים ארגוניים בלבד מאפליקציות המנוהלות על-ידי Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [מחיקת כל הנתונים ממכשיר macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).