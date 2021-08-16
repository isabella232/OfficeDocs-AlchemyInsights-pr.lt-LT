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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002128"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia attributeValueMustBeUnique klaidos priežastis yra du objektai, kurių sourceAnchor (immutableId) turi tą pačią reikšmę ProxyAddresses ir (arba) UserPrincipalName atributams. Norėdami ištaisyti klaidą AttributeValueMustBeUnique:
  
1. Identifikuokite dubliuotas proxyAddresses, userPrincipalName arba kitą atributo reikšmę, dėl kurios kyla klaida. Taip pat nustatykite, kurie du (ar daugiau) objektų yra susiję su konfliktu. Ataskaita, sugeneruota "Azure AD Prisijungimas Health", kad būtų galima sinchronizuoti, gali padėti nustatyti du objektus.
    
2. Nustatykite, kuris objektas ir toliau turi turėti dubliuotas reikšmę, o kurio objekto neturėtų būti.
    
3. Pašalinkite dubliuotas reikšmę iš objekto, kuriame neturėtų būti šios reikšmės. Atkreipkite dėmesį, kad turite pakeisti katalogą, iš kur objektas yra iš jo šaltinio. Kai kuriais atvejais gali tekti panaikinti vieną iš nesuderinamų objektų.
    
4. Jei atlikote pakeitimą vietiniame AD, leiskite "Azure AD Prisijungimas sinchronizuoti klaidos pakeitimą, kad būtų išspręstas.
    

