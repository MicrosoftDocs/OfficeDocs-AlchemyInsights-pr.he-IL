---
title: פתרון בעיות של הודעות נדחתה על-ידי Access
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760342"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>פתרון בעיות של הודעות נדחתה על-ידי Access במרכז הניהול של Sharepoint/OneDrive

אם אתה מקבל הודעה שהגישה נדחתה בעת ניסיון לבצע עיון למרכז הניהול של Sharepoint/OneDrive, נא ודא כי זה [רשיון למשתמש הקצה](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). אם למשתמש יש רשיון, עליך לוודא גם שהם [להקצות תפקיד מנהל](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) יכולים לגשת אליהם מרכזי admin.

בעיה זו עלולה להתרחש גם כאשר המשתמש יימחק וייווצר מחדש עם אותו השם העיקרי של המשתמש (UPN). החשבון החדש נוצר באמצעות ערך ה-PUID (מזהה ייחודי של Passport) שונה. כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive שלהם, יש למשתמש של ה-PUID שגוי. תרחיש השני כרוך סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם יש כבר נכנסו ל- SharePoint, ולאחר מכן הם הועברו לתפריט OU שונים ומשתמשים resynced עם SharePoint, עלול להיתקל בבעיה זו.

כדי לפתור בעיה זו, שחזר את UPN המקורי עם השלבים במאמר, [שחזור משתמש ב- Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

הערה: אם מרכז OneDrive או הניהול של SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שקיימת בעיית שירות זמניים.  [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).

