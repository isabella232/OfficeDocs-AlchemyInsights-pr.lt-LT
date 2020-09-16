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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor elgesys

"Azure AD Connect" (versijos 1.1.524.0 ir po) dabar palengvina KRS pažeidimų naudojimą kaip sourceAnchor atributą. Naudojant šią funkciją, "Azure AD Connect" automatiškai konfigūruoja sinchronizavimo taisykles:
  
- Naudoti KRS-ConsistencyGuid kaip vartotojo objektų sourceAnchor atributą. ObjectGUID naudojamas kitų tipų objektams.
    
- Į bet kurį vietinį skelbimo vartotojo objektą, kurio msDS-ConsistencyGuid atributas neužpildomas, "Azure AD Connect" įrašo savo objectGUID reikšmę atgal į KRS-ConsistencyGuid atributą vietiniame "Active Directory". Po to, kai "msDS-ConsistencyGuid" atributas yra užpildomas, "Azure AD Connect" eksportuos objektą į "Azure AD".
    
 **Pastaba:** Kai vietinis skelbimo objektas importuojamas į "Azure AD Connect" (tai yra importuotas į skelbimų jungties sritį ir projektuojamas į "metaverse"), negalite pakeisti jo sourceAnchor reikšmės. Norėdami nurodyti duoto vietinio skelbimo objekto sourceAnchor reikšmę, sukonfigūruokite jos KRS-ConsistencyGuid atributą, prieš importuodami į "Azure AD Connect". 
  
Daugiau informacijos apie SourceAnchor ir ConsistencyGuid rasite toliau pateiktoje lentelėje: " [AZURE AD Connect": dizaino koncepcijos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

