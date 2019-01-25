---
title: Klaidos AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499642"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia AttributeValueMustBeUnique klaida priežastis du objektus su skirtingų SourceAnchor (immutableId) turi tą pačią vertę dėl ProxyAddresses ir (arba) UserPrincipalName atributus. Nustatyti AttributeValueMustBeUnique klaida:
  
1. Nustatyti besidubliuojančių proxyAddresses, userPrincipalName ar kitų atributo reikšmė, kuri kyla problema. Taip pat nurodyti, kurių dvi (ar daugiau) objektų yra įtrauktos į konfliktą. Į pranešimą generuoja Azure AD Connect sveikatos Sync gali padėti jums nustatyti du objektai.
    
2. Nustatyti, kuris objektas turėtų ir toliau turėti dvigubą reikšmę ir koks objektas neturėtų būti.
    
3. Pašalinti dvigubą reikšmę iš objekto, kad neturėtų reikšmės. Atkreipkite dėmesį, kad jums turėtų atlikti pakeitimus į katalogą, kur objektas yra gaunama iš. Kai kuriais atvejais gali tekti panaikinti vieną iš konflikto objektus.
    
4. Jei pakeitimų autorių apie patalpose skelbimų, tegul Azure AD Connect Sinchronizavimo klaidos gauti fiksuoto kaita.
    

