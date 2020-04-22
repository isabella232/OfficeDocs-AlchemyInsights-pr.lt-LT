---
title: ConsistencyGuid / sourceAnchor veikimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705741"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor veikimas

Azure AD Connect (1.1.524.0 ir po versija) dabar palengvina msDS-ConsistencyGuid kaip sourceAnchor atributas naudoti. Naudojant šią funkciją, Azure AD Connect automatiškai konfigūruoja sinchronizavimo taisykles:
  
- Naudoti msDS-ConsistencyGuid kaip atributą sourceAnchor vartotojo objektų. ObjectGUID naudojamas kitų tipų objektams.
    
- Bet kurį vietinį AD vartotojo objektą, kurio msDS-ConsistencyGuid atributas neužpildomas, Azure AD Connect rašo savo objectGUID reikšmę atgal į atributą msDS-ConsistencyGuid vietiniame Active Directory. Po to, kai msDS-ConsistencyGuid atributas yra užpildytas, Azure AD Connect tada eksportuoja objektą azure AD.
    
 **Pastaba:** Kai vietiniame AD objektas yra importuojami į Azure AD Connect (t. y. importuoti į AD jungtis vietos ir projektuojami į metaverse), negalite pakeisti savo sourceAnchor reikšmė anymore. Norėdami nurodyti nurodyto vietinio AD objekto sourceAnchor reikšmę, sukonfigūruokite atributą msDS-ConsistencyGuid prieš jį importuodami į "Azure AD Connect". 
  
Jei norite gauti daugiau informacijos apie SourceAnchor ir ConsistencyGuid, ieškokite šioje: [Azure AD Connect: dizaino sąvokos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

