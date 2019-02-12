---
title: Klaidos AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916532"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia AttributeValueMustBeUnique klaida priežastis du objektus su skirtingų SourceAnchor (immutableId) turi tą pačią vertę dėl ProxyAddresses ir (arba) UserPrincipalName atributus. Nustatyti AttributeValueMustBeUnique klaida:
  
1. Nustatyti besidubliuojančių proxyAddresses, userPrincipalName ar kitų atributo reikšmė, kuri kyla problema. Taip pat nurodyti, kurių dvi (ar daugiau) objektų yra įtrauktos į konfliktą. Į pranešimą generuoja Azure AD Connect sveikatos Sync gali padėti jums nustatyti du objektai.
    
2. Nustatyti, kuris objektas turėtų ir toliau turėti dvigubą reikšmę ir koks objektas neturėtų būti.
    
3. Pašalinti dvigubą reikšmę iš objekto, kad neturėtų reikšmės. Atkreipkite dėmesį, kad jums turėtų atlikti pakeitimus į katalogą, kur objektas yra gaunama iš. Kai kuriais atvejais gali tekti panaikinti vieną iš konflikto objektus.
    
4. Jei pakeitimų autorių apie patalpose skelbimų, tegul Azure AD Connect Sinchronizavimo klaidos gauti fiksuoto kaita.
    

