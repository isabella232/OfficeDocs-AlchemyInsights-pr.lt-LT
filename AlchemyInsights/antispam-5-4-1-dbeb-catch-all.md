---
title: AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707919"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="003be-102">Problemos, susijusios su klaidos kodu 550 5.4.1 Perdavimo prieiga uždrausta, sprendimas</span><span class="sxs-lookup"><span data-stu-id="003be-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="003be-103">Ši problema kyla, kai [patikrinti, ar el. pašto adresas galioja siekiant išvengti bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) įvedant "Microsoft" tinklą.</span><span class="sxs-lookup"><span data-stu-id="003be-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="003be-104">Pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="003be-104">Try the following:</span></span>

1. <span data-ttu-id="003be-105">Nustatykite, ar problema būdinga visam domenui, ar vienam el. pašto adresui:</span><span class="sxs-lookup"><span data-stu-id="003be-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="003be-106">Visas domenas: kartais domeną reikia sinchronizuoti; pabandykite [nustatyti domeno vidinis ir tada atgal į patikimą](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="003be-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="003be-107">Vienas el. pašto adresas: Kartais adresą reikia sinchronizuoti; pakeisti smtp tarpinio serverio adresą ir tada jį pakeisti atgal gali padėti.</span><span class="sxs-lookup"><span data-stu-id="003be-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="003be-108">Nustatykite, ar problema būdinga grupei, ar viešajam aplankui.</span><span class="sxs-lookup"><span data-stu-id="003be-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="003be-109">Kai kurių tipų objektams gali tekti rankiniu būdu sukurti "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="003be-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="003be-110">Jei jums reikia papildomos pagalbos, atidarykite palaikymo bilietą ir nurodykite problemos apimtį (įskaitant objekto, kuriam siunčiate, tipą), kad galėtume jums padėti geriau.</span><span class="sxs-lookup"><span data-stu-id="003be-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>