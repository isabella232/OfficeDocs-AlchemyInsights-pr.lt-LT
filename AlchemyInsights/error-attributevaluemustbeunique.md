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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402711"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia AttributeValueMustBeUnique klaida priežastis du objektus su skirtingų SourceAnchor (immutableId) turi tą pačią vertę dėl ProxyAddresses ir (arba) UserPrincipalName atributus. Nustatyti AttributeValueMustBeUnique klaida:
  
1. Nustatyti besidubliuojančių proxyAddresses, userPrincipalName ar kitų atributo reikšmė, kuri kyla problema. Taip pat nurodyti, kurių dvi (ar daugiau) objektų yra įtrauktos į konfliktą. Į pranešimą generuoja Azure AD Connect sveikatos Sync gali padėti jums nustatyti du objektai.
    
2. Nustatyti, kuris objektas turėtų ir toliau turėti dvigubą reikšmę ir koks objektas neturėtų būti.
    
3. Pašalinti dvigubą reikšmę iš objekto, kad neturėtų reikšmės. Atkreipkite dėmesį, kad jums turėtų atlikti pakeitimus į katalogą, kur objektas yra gaunama iš. Kai kuriais atvejais gali tekti panaikinti vieną iš konflikto objektus.
    
4. Jei pakeitimų autorių apie patalpose skelbimų, tegul Azure AD Connect Sinchronizavimo klaidos gauti fiksuoto kaita.
    

