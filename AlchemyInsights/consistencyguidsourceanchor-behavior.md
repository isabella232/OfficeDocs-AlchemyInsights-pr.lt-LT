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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

"Azure AD Connect" (1.1.524.0 ir naujesnė versija) dabar palengvina msDS-ConsistencyGuid kaip sourceAnchor atributo naudojimą. Naudojant šią funkciją, "Azure AD Connect" automatiškai konfigūruoja sinchronizavimo taisykles, kad:
  
- Naudokite msDS-ConsistencyGuid kaip sourceAnchor atributą vartotojo objektams. ObjectGUID naudojamas kitiems objektų tipams.
    
- Bet kurio vietinio AD vartotojo objekto, kurio atributas msDS-ConsistencyGuid neužpildomas, atveju "Azure AD Connect" įrašo objektoGUID reikšmę į msDS-ConsistencyGuid atributą vietinėje "Active Directory". Įvedus atributą msDS-ConsistencyGuid, "Azure AD Connect" eksportuoja objektą į "Azure AD".
    
 **Pastaba:** Kai vietinis AD objektas importuojamas į "Azure AD Connect" (t. y. importuotas į "AD Connector Space" ir suprojektuojamas į metaversą), nebegalite pakeisti jo sourceAnchor reikšmės. Norėdami nurodyti vietinio AD objekto reikšmę sourceAnchor, sukonfigūruokite jo msDS-ConsistencyGuid atributą prieš jį importuokite į "Azure AD Connect". 
  
Daugiau informacijos apie "SourceAnchor" ir "ConsistencyGuid" žr.: ["Azure AD Connect": dizaino sąvokos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

