---
title: AntiSpam 5.4.1 DBEB sugavimo-visi
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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672441"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f5fad-102">Nustatyti pristatymo problemos klaidos kodas 550 5.4.1 relės prieiga uždrausta</span><span class="sxs-lookup"><span data-stu-id="f5fad-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f5fad-103">Ši problema kyla [tikrinant, ar el. pašto adresas galioja išvengti bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) įvesdami Office 365 tinklo.</span><span class="sxs-lookup"><span data-stu-id="f5fad-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="f5fad-104">Išbandykite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="f5fad-104">Try the following:</span></span>

1. <span data-ttu-id="f5fad-105">Nustatyti, ar problema yra susijusi su visu domenu arba vienu el. pašto adresu:</span><span class="sxs-lookup"><span data-stu-id="f5fad-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f5fad-106">Visas domenas: kartais domeną reikia sinchronizuoti; Pabandykite [nustatyti domeną į vidaus ir tada atgal į autoritetingas](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="f5fad-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f5fad-107">Vienas el. pašto adresas: kartais reikia sinchronizuoti adresą; keičiant SMTP tarpinio serverio adresą ir tada keičiant jį atgal gali padėti.</span><span class="sxs-lookup"><span data-stu-id="f5fad-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f5fad-108">Nustatykite, ar problema yra susijusi su grupe ar viešuoju aplanku.</span><span class="sxs-lookup"><span data-stu-id="f5fad-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f5fad-109">Kai kurių objektų tipų objektai gali reikėti neautomatiniu būdu sukurti "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="f5fad-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f5fad-110">Jei jums reikia papildomos pagalbos, prašome atidaryti pagalbinį bilietą ir nurodyti problemos apimtį (includidng objekto, kurį siunčiate, tipą), kad galėtume jums padėti geriau.</span><span class="sxs-lookup"><span data-stu-id="f5fad-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>