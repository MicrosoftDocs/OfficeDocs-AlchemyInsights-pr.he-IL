---
title: הגבל גישה ב- SharePoint או OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759082"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>הגבל גישה ב- SharePoint או OneDrive

קיימות דרכים רבות כדי להגביל גישה אל שירותי SharePoint Online/OneDrive. השיטות השונות של הגבלת גישה המתוארות להלן. 

הגבלת הרשאה

ב- SharePoint Online ו OneDrive עבור העסק, אנו להגביל גישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי הענקת גישה אלה הקבוצות/יחידים יש להם גישה בלבד.

[התאמה אישית של הרשאות עבור SharePoint רשימה או ספריה](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[להתאים אישית הרשאות באתר SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[לשנות את ההרשאות של תיקיית משנה](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[בקרת גישה ממכשירים לא מנוהלים](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint או מנהל כללי ב- Office 365, באפשרותך לחסום או להגביל את הגישה לתוכן SharePoint ו- OneDrive ממכשירים לא מנוהל (אלה לא היברידית AD המצורפים או תואם ב- Intune).

הגבלת מיקום רשת

כמנהל IT, תוכל לשלוט בגישה למשאבי SharePoint ו- OneDrive בהתבסס על מיקומי הרשת המוגדרות שאתה נותן בהם אמון. פעולה זו מכונה גם מדיניות המבוססת על מיקום. לקבלת מידע נוסף, נא עיין [בקרה על גישה מקוונת של SharePoint ונתונים OneDrive בהתבסס על מיקום הרשת](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

הגבלת נעילה של האתר 

בתוך SharePoint Online לך את היכולת לנעול אוסף אתרים, כך שאף אחד יש גישה. מאפיין זה מוגדר באמצעות PowerShell [SharePoint מעטפת ניהול מקוון](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) באמצעות המאפיין [ערכת-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.

הגבל משתמשים ליצור אתרים או אתרי משנה

הניהול של SharePoint או הניהול הכללי של Office 365, באפשרותך לאפשר למשתמשים ליצור, לנהל אתרי SharePoint משלהם, לקבוע איזה סוג של אתרים שהם יכולים ליצור, וציין את מיקום האתרים. לקבלת מידע נוסף, ראה [יצירת אתר ניהול ב- SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)
