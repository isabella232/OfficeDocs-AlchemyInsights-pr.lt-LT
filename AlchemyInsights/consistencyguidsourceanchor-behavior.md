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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408116"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor elgesį

Žydros AD Connect (versijos 1.1.524.0 ir po) dabar galima naudoti SDL-ConsistencyGuid kaip sourceAnchor atributo. Naudojant šią funkciją, Azure AD Connect automatiškai sukonfigūruoja sinchronizavimo taisyklės:
  
- SDL-ConsistencyGuid naudoti vartotojo objektų kaip sourceAnchor atributo. Vartotojo vietinio vartojamas kitų objektų tipai.
    
- Bet kuriai vietinėje AD vartotojo objekto, kurio SDL-ConsistencyGuid atributas yra ne apgyvendintos, Azure AD Connect rašo savo vartotojo vietinio vertės atgal į KRS pažeidimų ConsistencyGuid atributą vietinės Active Directory. Po to, kai yra gyventojų KRS pažeidimų ConsistencyGuid atributą, tada Azure AD Connect eksporto objektas Azure AD.
    
 **Pastaba:** Kai vietinės reklamos objekto yra importuojama į Azure AD Connect (t. y. importuojami į skelbimų jungties srities ir prognozuojama į Metaverse), negalite keisti jo sourceAnchor reikšmė nebėra. Nurodyti sourceAnchor reikšmė yra suteikta vietinėje AD objekto, konfigūruoti savo KRS pažeidimų ConsistencyGuid atributą, kol ji yra importuojama į Azure AD Connect. 
  
Daugiau informacijos apie SourceAnchor ir ConsistencyGuid, kreiptis į šiuos: [Azure AD Connect: dizaino koncepcijas,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

