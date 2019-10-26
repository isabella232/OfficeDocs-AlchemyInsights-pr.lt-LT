---
title: Klaida AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36527024"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia priežastis, dėl AttributeValueMustBeUnique klaida yra du objektai su skirtingais SourceAnchor (immutableId) turi tą pačią reikšmę ProxyAddresses ir/arba UserPrincipalName atributus. Norėdami nustatyti AttributeValueMustBeUnique klaida:
  
1. Nustatyti dubliuoti proxyAddresses, userPrincipalName arba kitos atributo reikšmės, kuri sukelia klaida. Taip pat nustatykite, kurie du (ar daugiau) objektai yra susiję su konfliktu. Azure AD Connect Health sinchronizavimo sugeneruota ataskaita gali padėti nustatyti du objektus.
    
2. Nustatyti, kuris objektas turėtų ir toliau turėti besidubliuojančių reikšmė ir kuris objektas neturėtų.
    
3. Pašalinkite nukopijuota reikšmę iš objekto, kuris neturėtų būti ta reikšmė. Įsidėmėkite, kad reikia pakeisti katalogą, iš kurio gaunamas objektas. Kai kuriais atvejais gali reikėti panaikinti vieną iš konfliktinių objektų.
    
4. Jei atlikote pakeitimus patalpose AD, leiskite Azure AD Connect sinchronizavimo pakeisti klaidos gauti fiksuotas.
    

