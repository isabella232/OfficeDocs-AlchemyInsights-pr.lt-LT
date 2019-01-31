---
title: ConsistencyGuid / sourceAnchor elgesį
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659599"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="2ba5c-102">ConsistencyGuid / sourceAnchor elgesį</span><span class="sxs-lookup"><span data-stu-id="2ba5c-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="2ba5c-p101">Žydros AD Connect (versijos 1.1.524.0 ir po) dabar galima naudoti SDL-ConsistencyGuid kaip sourceAnchor atributo. Naudojant šią funkciją, Azure AD Connect automatiškai sukonfigūruoja sinchronizavimo taisyklės:</span><span class="sxs-lookup"><span data-stu-id="2ba5c-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="2ba5c-p102">SDL-ConsistencyGuid naudoti vartotojo objektų kaip sourceAnchor atributo. Vartotojo vietinio vartojamas kitų objektų tipai.</span><span class="sxs-lookup"><span data-stu-id="2ba5c-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="2ba5c-p103">Bet kuriai vietinėje AD vartotojo objekto, kurio SDL-ConsistencyGuid atributas yra ne apgyvendintos, Azure AD Connect rašo savo vartotojo vietinio vertės atgal į KRS pažeidimų ConsistencyGuid atributą vietinės Active Directory. Po to, kai yra gyventojų KRS pažeidimų ConsistencyGuid atributą, tada Azure AD Connect eksporto objektas Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2ba5c-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="2ba5c-p104">**Pastaba:** Kai vietinės reklamos objekto yra importuojama į Azure AD Connect (t. y. importuojami į skelbimų jungties srities ir prognozuojama į Metaverse), negalite keisti jo sourceAnchor reikšmė nebėra. Nurodyti sourceAnchor reikšmė yra suteikta vietinėje AD objekto, konfigūruoti savo KRS pažeidimų ConsistencyGuid atributą, kol ji yra importuojama į Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2ba5c-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="2ba5c-111">Daugiau informacijos apie SourceAnchor ir ConsistencyGuid, kreiptis į šiuos: [Azure AD Connect: dizaino koncepcijas,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="2ba5c-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

