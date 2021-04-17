---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821455"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="43184-102">Klaidos kodo 550 5.4.1 Perdavimo prieiga uždrausta pristatymo problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="43184-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="43184-103">Ši problema kyla [tikrinant, ar el. pašto adresas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) galioja, kad nebūtų sugrįžta įvedant "Microsoft" tinklą.</span><span class="sxs-lookup"><span data-stu-id="43184-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="43184-104">Išbandykite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="43184-104">Try the following:</span></span>

1. <span data-ttu-id="43184-105">Nustatykite, ar problema susijusi su visu domenu, ar vienu el. pašto adresu:</span><span class="sxs-lookup"><span data-stu-id="43184-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="43184-106">Visas domenas: kartais domeną reikia sinchronizuoti; pabandykite [nustatyti domeną kaip Vidinis, tada grįžkite į Patikimas](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="43184-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="43184-107">Vienas el. pašto adresas: kartais adresą reikia sinchronizuoti; pakeisti SMTP tarpinio serverio adresą ir tada jį pakeisti atgal gali padėti.</span><span class="sxs-lookup"><span data-stu-id="43184-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="43184-108">Nustatykite, ar problema susijusi su grupe ar viešuoju aplanku.</span><span class="sxs-lookup"><span data-stu-id="43184-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="43184-109">Kai kurių tipų objektus gali tekti rankiniu būdu sukurti "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="43184-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="43184-110">Jei reikia papildomos pagalbos, atidarykite palaikymo kvitą ir nurodykite problemos aprėptį (įskaitant objekto, į kurį siunčiate, tipą), kad galėtume jums padėti geriau.</span><span class="sxs-lookup"><span data-stu-id="43184-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>