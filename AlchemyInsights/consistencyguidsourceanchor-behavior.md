---
title: ConsistencyGuid / sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817000"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="7c45e-102">ConsistencyGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="7c45e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="7c45e-103">"Azure AD Connect" (1.1.524.0 ir naujesnė versija) dabar palengvina msDS-ConsistencyGuid kaip sourceAnchor atributo naudojimą.</span><span class="sxs-lookup"><span data-stu-id="7c45e-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="7c45e-104">Naudojant šią funkciją, "Azure AD Connect" automatiškai konfigūruoja sinchronizavimo taisykles, kad:</span><span class="sxs-lookup"><span data-stu-id="7c45e-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="7c45e-105">Naudokite msDS-ConsistencyGuid kaip sourceAnchor atributą vartotojo objektams.</span><span class="sxs-lookup"><span data-stu-id="7c45e-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="7c45e-106">ObjectGUID naudojamas kitiems objektų tipams.</span><span class="sxs-lookup"><span data-stu-id="7c45e-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="7c45e-107">Bet kurio vietinio AD vartotojo objekto, kurio atributas msDS-ConsistencyGuid neužpildomas, atveju "Azure AD Connect" įrašo objektoGUID reikšmę į msDS-ConsistencyGuid atributą vietinėje "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="7c45e-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="7c45e-108">Įvedus atributą msDS-ConsistencyGuid, "Azure AD Connect" eksportuoja objektą į "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="7c45e-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="7c45e-109">**Pastaba:** Kai vietinis AD objektas importuojamas į "Azure AD Connect" (t. y. importuotas į "AD Connector Space" ir suprojektuojamas į metaversą), nebegalite pakeisti jo sourceAnchor reikšmės.</span><span class="sxs-lookup"><span data-stu-id="7c45e-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="7c45e-110">Norėdami nurodyti vietinio AD objekto reikšmę sourceAnchor, sukonfigūruokite jo msDS-ConsistencyGuid atributą prieš jį importuokite į "Azure AD Connect".</span><span class="sxs-lookup"><span data-stu-id="7c45e-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="7c45e-111">Daugiau informacijos apie "SourceAnchor" ir "ConsistencyGuid" žr.: ["Azure AD Connect": dizaino sąvokos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="7c45e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

