---
title: פתרון בעיות בפריסת אישור של אימות לקוח
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555309"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="4e733-102">פתרון בעיות בפריסת אישור של אימות לקוח</span><span class="sxs-lookup"><span data-stu-id="4e733-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="4e733-103">פרופילי אישורי לקוח Intune NDES/SCEP ו-PKCS/PFX משמשים בדרך כלל בשילוב עם סוגי פרופילים אחרים כגון Wifi, VPN ודוא ל כדי לאפשר למשתמשים לבצע אימות למשאבי החברה.</span><span class="sxs-lookup"><span data-stu-id="4e733-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="4e733-104">כאשר סוגי פרופילים אלה מקושרים לפרופיל של אישור לקוח תלויים בפריסה המוצלחת של פרופיל זה.</span><span class="sxs-lookup"><span data-stu-id="4e733-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="4e733-105">הגדרת תשתית ראשונית ותצורה משויכת של הפרופיל של אישור הלקוח דורשות לעתים קרובות פתרון בעיות.</span><span class="sxs-lookup"><span data-stu-id="4e733-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="4e733-106">לקבלת מדריך שלב אחר שלב לכיוונון מוצלח של מחבר NDES ולפתרון בעיות הדרכה לבידוד בעיות בפריסת האישורים, ראה:</span><span class="sxs-lookup"><span data-stu-id="4e733-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="4e733-107">קביעת תצורה של תשתית לתמיכה ב-SCEP עם Intune</span><span class="sxs-lookup"><span data-stu-id="4e733-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="4e733-108">סקירה כללית של פתרון בעיות בפרופילי אישורים של SCEP עם Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4e733-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="4e733-109">השתמש בסקריפטים שאליהם מפנה powershell כדי לסייע באימות התצורה.</span><span class="sxs-lookup"><span data-stu-id="4e733-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="4e733-110">לקבלת מידע נוסף, ראה [Intune סקריפטים לאימות מחבר אישור](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="4e733-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="4e733-111">**סוגיות נפוצות אחרות**</span><span class="sxs-lookup"><span data-stu-id="4e733-111">**Other common issues**</span></span>

<span data-ttu-id="4e733-112">**כאשר אני מנסה להתקין את מחבר האישור Intune בשרת המחבר NDES, אני מקבל את ההודעה "אין אפשרות לאמת את הסיסמה בבקשת האישור. . ייתכן שכבר השתמשו בו השג סיסמה חדשה לשליחה באמצעות בקשה זו. "**</span><span class="sxs-lookup"><span data-stu-id="4e733-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="4e733-113">הודעה זו פירושה שעליך להפעיל את התקנת מחבר האישורים כמנהל.</span><span class="sxs-lookup"><span data-stu-id="4e733-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="4e733-114">בסביבות מסוימות, השרתים שבהם האישור Intune פועל חייבים להשתמש בשרת proxy כדי להתחבר ל-Intune ולכן מחבר האישורים חייב להשתמש ב-proxy.</span><span class="sxs-lookup"><span data-stu-id="4e733-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="4e733-115">בנסיבות מסוימות, מחבר NDES מתעלם מהגדרות ה-proxy שהוגדרו וייתכן שיהיה צורך לקבוע את תצורת הגדרות ה-proxy בעת הפעלה בהקשר האבטחה של LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="4e733-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="4e733-116">הפתרון הוא להפעיל את Internet Explorer כמערכת ולהגדיר proxy ב-IE.</span><span class="sxs-lookup"><span data-stu-id="4e733-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="4e733-117">לאחר הפעלה מחדש של שירות מחבר Intune, מחבר NDES מתחבר לIntune.</span><span class="sxs-lookup"><span data-stu-id="4e733-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="4e733-118">**התקני משתמש אינם מקבלים עוד אישורי SCEP מ-NDES.**</span><span class="sxs-lookup"><span data-stu-id="4e733-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="4e733-119">ייתכן שאישור אימות הלקוח הונפק לשרת NDES ושצוין במהלך התקנת מחבר NDES, פג תוקפו או שחסר.</span><span class="sxs-lookup"><span data-stu-id="4e733-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="4e733-120">כדי לפתור:</span><span class="sxs-lookup"><span data-stu-id="4e733-120">To resolve:</span></span> 
 
1. <span data-ttu-id="4e733-121">הסר את ההתקנה של מחבר NDES.</span><span class="sxs-lookup"><span data-stu-id="4e733-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="4e733-122">השתמש בפרטים אלה כדי לבקש אימות חדש של לקוח או אישור אימות שרת:</span><span class="sxs-lookup"><span data-stu-id="4e733-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="4e733-123">שם הנושא: CN = fqdn חיצוני</span><span class="sxs-lookup"><span data-stu-id="4e733-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="4e733-124">שם חלופי של נושא (שניהם נדרשים): DNS = fqdn חיצוני, DNS = fqdn פנימי</span><span class="sxs-lookup"><span data-stu-id="4e733-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="4e733-125">התקן מחדש את מחבר NDES באישור החדש.</span><span class="sxs-lookup"><span data-stu-id="4e733-125">Reinstall the NDES connector with the new certificate.</span></span>