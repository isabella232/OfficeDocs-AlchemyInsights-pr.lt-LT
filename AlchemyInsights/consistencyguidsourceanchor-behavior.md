---
title: ConsistencyGuid/sourceAnchor veikimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516998"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d1071-102">ConsistencyGuid/sourceAnchor veikimas</span><span class="sxs-lookup"><span data-stu-id="d1071-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d1071-103">Azure AD Connect (versija 1.1.524.0 ir po) dabar palengvina msDS-ConsistencyGuid kaip sourceAnchor atributo naudojimą.</span><span class="sxs-lookup"><span data-stu-id="d1071-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d1071-104">Naudojant šią funkciją, Azure AD Connect automatiškai sukonfigūruoja sinchronizavimo taisykles, kad:</span><span class="sxs-lookup"><span data-stu-id="d1071-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d1071-105">Naudokite msDS-ConsistencyGuid kaip vartotojo objektų sourceAnchor atributą.</span><span class="sxs-lookup"><span data-stu-id="d1071-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d1071-106">ObjectGUID naudojamas kitiems objekto tipams.</span><span class="sxs-lookup"><span data-stu-id="d1071-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d1071-107">Bet kuriuo metu vietinio AD vartotojo objekto, kurio msDS-ConsistencyGuid atributas nėra apgyvendintos, Azure AD Connect rašo savo objectGUID reikšmę į msDS-ConsistencyGuid atributas vietinėje Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1071-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d1071-108">Po to, kai msDS-ConsistencyGuid atributas yra paruoštą, Azure AD Connect tada eksportuoti objektą į Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1071-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d1071-109">**Pastaba:** Kai vietinio AD objekto importuojamas į Azure AD Connect (t. y. importuoti į AD jungties vietos ir prognozuojama į Metaverse), jūs negalite pakeisti savo sourceAnchor reikšmė nebėra.</span><span class="sxs-lookup"><span data-stu-id="d1071-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d1071-110">Norėdami nurodyti "sourceAnchor" reikšmę, nurodytą vietinėje AD objekte, prieš importuodama į "Azure AD Connect" sukonfigūruokite atributą msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="d1071-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d1071-111">Daugiau informacijos apie SourceAnchor ir ConsistencyGuid, ieškokite šioje: [AZURE AD Connect: dizaino koncepcijos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d1071-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

