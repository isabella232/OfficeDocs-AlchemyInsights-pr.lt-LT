---
title: ConsistencyGuid / sourceAnchor elgesį
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516998"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="6f459-102">ConsistencyGuid / sourceAnchor elgesį</span><span class="sxs-lookup"><span data-stu-id="6f459-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="6f459-103">Žydros AD Connect (versijos 1.1.524.0 ir po) dabar galima naudoti SDL-ConsistencyGuid kaip sourceAnchor atributo.</span><span class="sxs-lookup"><span data-stu-id="6f459-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="6f459-104">Naudojant šią funkciją, Azure AD Connect automatiškai sukonfigūruoja sinchronizavimo taisyklės:</span><span class="sxs-lookup"><span data-stu-id="6f459-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="6f459-105">SDL-ConsistencyGuid naudoti vartotojo objektų kaip sourceAnchor atributo.</span><span class="sxs-lookup"><span data-stu-id="6f459-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="6f459-106">Vartotojo vietinio vartojamas kitų objektų tipai.</span><span class="sxs-lookup"><span data-stu-id="6f459-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="6f459-107">Bet kuriai vietinėje AD vartotojo objekto, kurio SDL-ConsistencyGuid atributas yra ne apgyvendintos, Azure AD Connect rašo savo vartotojo vietinio vertės atgal į KRS pažeidimų ConsistencyGuid atributą vietinės Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6f459-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="6f459-108">Po to, kai yra gyventojų KRS pažeidimų ConsistencyGuid atributą, tada Azure AD Connect eksporto objektas Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f459-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="6f459-109">**Pastaba:** Kai vietinės reklamos objekto yra importuojama į Azure AD Connect (t. y. importuojami į skelbimų jungties srities ir prognozuojama į Metaverse), negalite keisti jo sourceAnchor reikšmė nebėra.</span><span class="sxs-lookup"><span data-stu-id="6f459-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="6f459-110">Nurodyti sourceAnchor reikšmė yra suteikta vietinėje AD objekto, konfigūruoti savo KRS pažeidimų ConsistencyGuid atributą, kol ji yra importuojama į Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6f459-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="6f459-111">Daugiau informacijos apie SourceAnchor ir ConsistencyGuid, kreiptis į šiuos: [Azure AD Connect: dizaino koncepcijas,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="6f459-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

