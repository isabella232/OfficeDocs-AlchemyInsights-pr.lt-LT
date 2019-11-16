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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516998"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor veikimas

Azure AD Connect (versija 1.1.524.0 ir po) dabar palengvina msDS-ConsistencyGuid kaip sourceAnchor atributo naudojimą. Naudojant šią funkciją, Azure AD Connect automatiškai sukonfigūruoja sinchronizavimo taisykles, kad:
  
- Naudokite msDS-ConsistencyGuid kaip vartotojo objektų sourceAnchor atributą. ObjectGUID naudojamas kitiems objekto tipams.
    
- Bet kuriuo metu vietinio AD vartotojo objekto, kurio msDS-ConsistencyGuid atributas nėra apgyvendintos, Azure AD Connect rašo savo objectGUID reikšmę į msDS-ConsistencyGuid atributas vietinėje Active Directory. Po to, kai msDS-ConsistencyGuid atributas yra paruoštą, Azure AD Connect tada eksportuoti objektą į Azure AD.
    
 **Pastaba:** Kai vietinio AD objekto importuojamas į Azure AD Connect (t. y. importuoti į AD jungties vietos ir prognozuojama į Metaverse), jūs negalite pakeisti savo sourceAnchor reikšmė nebėra. Norėdami nurodyti "sourceAnchor" reikšmę, nurodytą vietinėje AD objekte, prieš importuodama į "Azure AD Connect" sukonfigūruokite atributą msDS-ConsistencyGuid. 
  
Daugiau informacijos apie SourceAnchor ir ConsistencyGuid, ieškokite šioje: [AZURE AD Connect: dizaino koncepcijos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

