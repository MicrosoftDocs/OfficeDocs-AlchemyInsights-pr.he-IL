---
title: תיקון יישומי Microsoft 365 מצטערים, אנו נתקלים בהודעה של בעיות שרת זמניות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835272"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>תיקון ההודעה של יישומי Microsoft 365 "מצטערים, אנחנו נתקלים בבעיות שרת זמניות"

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את הגדרות חומת האש, תוכנת האנטי-וירוס וה- Proxy כדי לוודא שהם אינם חוסמים גישה לאינטרנט לאפליקציות Microsoft 365. ראה [כתובות URL וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. עבור אל  >  **התחל הפעלה** ולאחר מכן הקלד **services.msc**. ודא שהשירותים הבאים פועלים כולם:
    - התקנה אוטומטית של מכשירים מחוברים לרשת
    - שירות רשימת רשת
    - המודעות למיקום ברשת
    - יומן האירועים של Windows

אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו. אם יש לך בעיה בה הפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:

**sfc /scannow**

לאחר סיום פקודה זו, הפעל מחדש את המחשב.

לקבלת מידע מפורט, [ראה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נא נסה שוב מאוחר יותר" שגיאה בעת הפעלת](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).