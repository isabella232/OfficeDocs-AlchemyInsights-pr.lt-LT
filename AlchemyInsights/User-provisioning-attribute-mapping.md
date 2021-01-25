---
title: Vartotojo parengimo atributo susiejimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949889"
---
# <a name="user-provisioning-attribute-mapping"></a>Vartotojo parengimo atributo susiejimas

1. Norėdami pašalinti žinomas atributų priskyrimo problemas, žiūrėkite [atributų susiejimų](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)nustatymas. 
2. "Microsoft Azure Active Directory" (AD) teikia vartotojų parengimo palaikymą trečiosios šalies "SaaS" programoms, pvz., Salesforce, G Suite ir kt. Jei įgalinate vartotojo parengimas trečiosios šalies "SaaS" taikomajai programai, "Azure" portalas kontroliuoja jo atributo reikšmes per atributų susiejimus. Norėdami sužinoti, kaip tinkinti numatytuosius atributų susiejimus, žiūrėkite [vartotojo parengimo atributų tinkinimas "Azure Active Directory" "SaaS" taikomosiose programose](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Norėdami sužinoti daugiau apie SaaS App vartotojo parengimą, žiūrėkite [kas yra automatizuota SaaS App vartotojo parengimas "AZURE AD"?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Tinkindami atributų susiejimus vartotojo parengimo tikslais, galite pastebėti, kad atributas, kurį norite priskirti, nerodomas šaltinio atributų sąraše. [Atributas sinchronizuoti iš jūsų vietinio "Active Directory" į "AZURE AD" dėl parengimo taikomosios programos](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) straipsnyje rodoma, kaip įtraukti trūkstamą atributą sinchronizuojant jį iš vietinio skelbimo į "Azure AD".
