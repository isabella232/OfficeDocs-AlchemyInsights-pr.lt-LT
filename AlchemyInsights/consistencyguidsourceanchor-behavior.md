---
title: ConsistencyGuid/sourceAnchor elgesys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756291"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="5c5b0-102">ConsistencyGuid/sourceAnchor elgesys</span><span class="sxs-lookup"><span data-stu-id="5c5b0-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="5c5b0-103">"Azure AD Connect" (versijos 1.1.524.0 ir po) dabar palengvina KRS pažeidimų naudojimą kaip sourceAnchor atributą.</span><span class="sxs-lookup"><span data-stu-id="5c5b0-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="5c5b0-104">Naudojant šią funkciją, "Azure AD Connect" automatiškai konfigūruoja sinchronizavimo taisykles:</span><span class="sxs-lookup"><span data-stu-id="5c5b0-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="5c5b0-105">Naudoti KRS-ConsistencyGuid kaip vartotojo objektų sourceAnchor atributą.</span><span class="sxs-lookup"><span data-stu-id="5c5b0-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="5c5b0-106">ObjectGUID naudojamas kitų tipų objektams.</span><span class="sxs-lookup"><span data-stu-id="5c5b0-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="5c5b0-107">Į bet kurį vietinį skelbimo vartotojo objektą, kurio msDS-ConsistencyGuid atributas neužpildomas, "Azure AD Connect" įrašo savo objectGUID reikšmę atgal į KRS-ConsistencyGuid atributą vietiniame "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="5c5b0-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="5c5b0-108">Po to, kai "msDS-ConsistencyGuid" atributas yra užpildomas, "Azure AD Connect" eksportuos objektą į "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="5c5b0-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="5c5b0-109">**Pastaba:** Kai vietinis skelbimo objektas importuojamas į "Azure AD Connect" (tai yra importuotas į skelbimų jungties sritį ir projektuojamas į "metaverse"), negalite pakeisti jo sourceAnchor reikšmės.</span><span class="sxs-lookup"><span data-stu-id="5c5b0-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="5c5b0-110">Norėdami nurodyti duoto vietinio skelbimo objekto sourceAnchor reikšmę, sukonfigūruokite jos KRS-ConsistencyGuid atributą, prieš importuodami į "Azure AD Connect".</span><span class="sxs-lookup"><span data-stu-id="5c5b0-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="5c5b0-111">Daugiau informacijos apie SourceAnchor ir ConsistencyGuid rasite toliau pateiktoje lentelėje: " [AZURE AD Connect": dizaino koncepcijos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="5c5b0-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

