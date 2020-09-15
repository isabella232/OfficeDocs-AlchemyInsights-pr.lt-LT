---
title: AntiSpam 5.4.1 DBEB catch-All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717369"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="5553d-102">Problemų, susijusių su klaidos kodu 550 5.4.1 Relay prieiga uždrausta, šalinimas</span><span class="sxs-lookup"><span data-stu-id="5553d-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="5553d-103">Ši problema kyla [tikrinant, ar el. pašto adresas galioja, kad būtų išvengta "bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) " įvedant "Microsoft" tinklą.</span><span class="sxs-lookup"><span data-stu-id="5553d-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="5553d-104">Išbandykite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="5553d-104">Try the following:</span></span>

1. <span data-ttu-id="5553d-105">Nustatykite, ar problema būdinga visam domenui, ar vienam elektroninio pašto adresui:</span><span class="sxs-lookup"><span data-stu-id="5553d-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="5553d-106">Visas domenas: kartais domeną reikia sinchronizuoti; Pabandykite [nustatyti domeną kaip vidinį ir grįžti į patikimą](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="5553d-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="5553d-107">Vienas elektroninio pašto adresas: kartais adresą reikia sinchronizuoti; pakeitus SMTP tarpinio serverio adresą ir pakeitus jį atgal, gali padėti.</span><span class="sxs-lookup"><span data-stu-id="5553d-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="5553d-108">Nustatykite, ar problema būdinga grupei ar viešajam aplankui.</span><span class="sxs-lookup"><span data-stu-id="5553d-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="5553d-109">Kai kurių objektų tipų objektams gali reikėti rankiniu būdu sukurti "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="5553d-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="5553d-110">Jei reikia papildomos pagalbos, atidarykite palaikymo bilietą ir nurodykite problemos aprėptį (įskaitant objekto, kurį siunčiate, tipą), kad galėtume jums padėti geriau.</span><span class="sxs-lookup"><span data-stu-id="5553d-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>