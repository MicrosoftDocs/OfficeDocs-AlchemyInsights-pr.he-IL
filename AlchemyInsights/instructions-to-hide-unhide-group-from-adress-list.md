---
title: הוראות להסתיר/לבטל הסתרה של קבוצה מרשימת כתובות
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831879"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>הסתרת קבוצת Microsoft 365 מרשימת כתובות (GAL)

כדי להסתיר קבוצה של Microsoft 365 מרשימות כתובות (GAL) של לקוחות Exchange (כגון Outlook או OWA), השתמש בפקודה הבאה במעטפת EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

כדי להסתיר את הקבוצה של Microsoft 365 מלהיות גלויה ללקוחות Exchange, השתמש בפקודה הבאה במעטפת EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

