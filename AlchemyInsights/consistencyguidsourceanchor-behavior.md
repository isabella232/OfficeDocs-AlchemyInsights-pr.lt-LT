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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044348"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

"Azure AD Prisijungimas (1.1.524.0 ir naujesnė versija) dabar palengvina msDS-ConsistencyGuid kaip sourceAnchor atributo naudojimą. Naudojant šią funkciją, "Azure AD Prisijungimas automatiškai konfigūruoja sinchronizavimo taisykles, kad:
  
- Naudokite msDS-ConsistencyGuid kaip sourceAnchor atributą vartotojo objektams. ObjectGUID naudojamas kitiems objektų tipams.
    
- Bet kurio vietinio AD vartotojo objekto, kurio atributas msDS-ConsistencyGuid neužpildomas, atveju "Azure AD Prisijungimas" įrašo objektoGUID reikšmę į msDS-ConsistencyGuid atributą vietinėje "Active Directory". Įvedus atributą msDS-ConsistencyGuid, "Azure AD Prisijungimas tada eksportuoja objektą į "Azure AD".
    
 **Pastaba:** Kai vietinis AD objektas importuojamas į "Azure AD Prisijungimas" (t. y. importuotas į AD jungties vietą ir suprojektuojamas į metaversą), nebesikeičiama jo sourceAnchor reikšmė. Norėdami nurodyti vietinio AD objekto sourceAnchor reikšmę, sukonfigūruokite jo msDS-ConsistencyGuid atributą prieš jį importuokite į "Azure AD Prisijungimas". 
  
Daugiau informacijos apie "SourceAnchor" ir "ConsistencyGuid" žr.: ["Azure AD Prisijungimas" dizaino sąvokos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

