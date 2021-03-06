---
title: הקצאת משאבים למשתמש
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481890"
---
# <a name="user-provisioning"></a>הקצאת משאבים למשתמש

- השתמש ביכולת [הקצאת](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) המשאבים לפי דרישה כדי להקצות משתמש ולקבל אבחון מפורט אודות השלבים שננקטו.
- כדי לפתור בעיות שאתה נתקל בהן בעת הקצאת משתמשים וקבוצות, עיין במדריך לפתרון בעיות [לא מוקצים משתמשים](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- אם אתה מבחין כי משתמשים אינם מוקצים, ראה [הקצאת יומנים (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) ב-תכלת Active DIRECTORY (AD). חפש ערכי יומן רישום הקשורים למשתמש ספציפי.
- הפעלה מחדש של הקצאת משאבים כדי לתפוס משתמשים שפיספסו במחזור הקצאה קודם.
- ייתכן שהמשתמש/הקבוצה לא הוקצו מכיוון שהשירות שלנו לא הספיק להעריך את המשתמש עדיין. סקור את ההדרכה למשך הזמן הדרוש לאספקה ולפס ההתקדמות בדף קביעת התצורה של הקצאת המשאבים. אם המצב היציב שצוין במקטע הפרטים הנוספים הוא לפני התאריך שבו המשתמש נוצר/עודכן/נמחק, משמעות הדבר היא שעדיין לא הערכנו את המשתמש. בתרחיש זה, הדבר הטוב ביותר לעשות הוא להמתין לסיום שירות הקצאת המשאבים. אם המצב היציב הושג, מומלץ לבצע הפעלה מחדש מממשק המשתמש בפורטל התכלת.
  - שים לב שהשירות שלנו מודע רק לשינויים במשתמש/בקבוצה במערכת המקור (תכלת Active Directory). אם משתמש/קבוצה מוסר ישירות ביישום (לדוגמה, ServiceNow), איננו מודעים לשינויים אלה ואינם מגלגלים אותו בחזרה בהתבסס על מצב המשתמש במערכת המקור. בתרחיש זה, מומלץ להחזיר את השינוי ישירות ביישום היעד.
- השירות שלנו העריך את המשתמש/הקבוצה וקבע שאין להקצות אותו:
  - אם הגדרת את הטווח למשתמשים ולקבוצות המוקצים, בדוק אם המשתמש/הקבוצה מוקצים ליישום.
  - אם המשתמש/הקבוצה מוקצים ליישום, ודא שהוא אינו מוקצה לתפקיד ברירת המחדל של access. לא ניתן להשתמש בתפקיד זה לצורך הקצאת משאבים.
  - אם הגדרת מסנן טווח המבוסס על תכונה, ודא שהמשתמש עומד בקריטריונים שציינת.
  - אם המשתמשים כבר קיימים במערכת היעד והמצב של המשתמש בהתאמת המקור והיעד, לא נעשה כל פעולה נוספת.
- השירות שלנו ניסה להקצות את המשתמש והוא נכשל. עבור תרחישים אלה, עיין בכרטיסיה פתרון בעיות והמלצות ביומני הקצאת המשאבים:
  - ייתכן שתכונה נדרשת במשתמש חסרה ב-תכלת Active Directory או שאינה תואמת לתבנית הנדרשת על-ידי יישום צד שלישי. לדוגמה, התכונה Country במשתמש עשויה להיות מוגדרת לארצות הברית כאשר היא אמורה להיות אנחנו.
  - התכונה היא תכונת ייחוס שאינה קיימת עדיין ביישום היעד. תכונה של ייחוס הקשרים היא תכונה המפנה לאובייקט אחר, לדוגמה, משתמש החבר בקבוצה. מזהה המשתמש נמצא בתכונה ' חבר ' של הקבוצה, אך ניתן לעבד אותו רק אם אובייקט המשתמש שהוא מצביע עליו כבר קיים.
