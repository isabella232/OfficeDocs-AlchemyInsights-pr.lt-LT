---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813768"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia attributeValueMustBeUnique klaidos priežastis yra du objektai, kurių sourceAnchor (immutableId) turi tą pačią reikšmę ProxyAddresses ir (arba) UserPrincipalName atributams. Norėdami ištaisyti klaidą AttributeValueMustBeUnique:
  
1. Identifikuokite dubliuotas proxyAddresses, userPrincipalName arba kitą atributo reikšmę, dėl kurios kyla klaida. Taip pat nustatykite, kurie du (ar daugiau) objektų yra susiję su konfliktu. "Azure AD Connect Health" sugeneruota ataskaita, skirta sinchronizuoti, gali padėti nustatyti du objektus.
    
2. Nustatykite, kuris objektas ir toliau turi turėti dubliuotas reikšmę, o kurio objekto neturėtų būti.
    
3. Pašalinkite dubliuotas reikšmę iš objekto, kuriame neturėtų būti šios reikšmės. Atkreipkite dėmesį, kad turite pakeisti katalogą, iš kur objektas yra iš jo šaltinio. Kai kuriais atvejais gali tekti panaikinti vieną iš nesuderinamų objektų.
    
4. Jei atlikote pakeitimą vietiniame AD, leiskite "Azure AD Connect" sinchronizuoti klaidos pakeitimą, kad būtų išspręstas.
    

