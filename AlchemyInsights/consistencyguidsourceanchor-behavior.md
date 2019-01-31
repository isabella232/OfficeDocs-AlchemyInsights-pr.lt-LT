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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor elgesį

Žydros AD Connect (versijos 1.1.524.0 ir po) dabar galima naudoti SDL-ConsistencyGuid kaip sourceAnchor atributo. Naudojant šią funkciją, Azure AD Connect automatiškai sukonfigūruoja sinchronizavimo taisyklės:
  
- SDL-ConsistencyGuid naudoti vartotojo objektų kaip sourceAnchor atributo. Vartotojo vietinio vartojamas kitų objektų tipai.
    
- Bet kuriai vietinėje AD vartotojo objekto, kurio SDL-ConsistencyGuid atributas yra ne apgyvendintos, Azure AD Connect rašo savo vartotojo vietinio vertės atgal į KRS pažeidimų ConsistencyGuid atributą vietinės Active Directory. Po to, kai yra gyventojų KRS pažeidimų ConsistencyGuid atributą, tada Azure AD Connect eksporto objektas Azure AD.
    
 **Pastaba:** Kai vietinės reklamos objekto yra importuojama į Azure AD Connect (t. y. importuojami į skelbimų jungties srities ir prognozuojama į Metaverse), negalite keisti jo sourceAnchor reikšmė nebėra. Nurodyti sourceAnchor reikšmė yra suteikta vietinėje AD objekto, konfigūruoti savo KRS pažeidimų ConsistencyGuid atributą, kol ji yra importuojama į Azure AD Connect. 
  
Daugiau informacijos apie SourceAnchor ir ConsistencyGuid, kreiptis į šiuos: [Azure AD Connect: dizaino koncepcijas,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

