---
title: Klaidos AtributValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703182"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia AtributValueMustBeUnique klaidos priežastis yra du objektai su skirtingais SourceAnchor (immutableId) turi tą pačią reikšmę ProxyAddresses ir (arba) UserPrincipalName atributams. Norėdami išspręsti AtributValueMustBeUnique klaida:
  
1. Nustatykite dubliuotą proxyAddresses, userPrincipalName arba kitą atributo reikšmę, dėl kurios įvyksta klaida. Taip pat nurodykite, kurie du (ar daugiau) objektai yra susiję su konfliktu. "Azure AD Connect Health" sinchronizavimo sugeneruota ataskaita gali padėti nustatyti du objektus.
    
2. Nustatyti, kuris objektas ir toliau turi dubliuotą reikšmę, o kuris objektas neturėtų būti.
    
3. Pašalinkite dubliuotą reikšmę iš objekto, kuris neturėtų turėti šios reikšmės. Atkreipkite dėmesį, kad turėtumėte pakeisti katalogą, iš kurio gaunamas objektas. Kai kuriais atvejais gali tekti panaikinti vieną iš konflikto objektų.
    
4. Jei atlikote pakeitimus vietoje AD, tegul Azure AD Connect sinchronizuoti pakeitimą klaida gauti išspręsti.
    

