---
title: Vartotojo parengimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481886"
---
# <a name="user-provisioning"></a>Vartotojo parengimas

- Naudokite [užsakomąsias parengimo](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) galimybes, kad suteiktumėte vartotojui ir gautumėte išsamią diagnostiką apie veiksmus, kurių imtasi.
- Norėdami pašalinti problemas, su kuriomis susidūrėte, kai konfigūruojami vartotojai ir grupės, peržiūrėkite trikčių diagnostikos vadovą [jokie vartotojai nėra konfigūruojami](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Jei pastebite, kad vartotojai nėra parengti, peržiūrėkite [parengimo žurnalus (peržiūra)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) "Azure Active Directory" (AD). Ieškoti žurnalų įrašų, susijusių su konkrečiu vartotoju.
- Periodiškai paleiskite parengimo programą, kad būtų sugauti visi vartotojai, kurie buvo praleisti ankstesnio parengimo ciklo metu.
- Vartotojas/grupė galėjo būti nesukonfigūruota, nes mūsų tarnyba dar neturėjo galimybės įvertinti vartotojo. Peržiūrėkite nurodymus, kaip ilgai trunka parengimas, taip pat ir eigos juostos parengimo konfigūravimo puslapyje. Jei stabili būsena, nurodyta sekcijoje papildoma informacija, yra prieš vartotojo sukūrimo/atnaujinimo/panaikinimo datą, tai reiškia, kad dar neįvertinome vartotojo. Pagal šį scenarijų, geriausia, ką reikia padaryti – palaukite, kol bus baigta parengimo tarnyba. Jei pasiekta pastovi būsena, rekomenduojame paleisti iš naujo nuo vartotojo sąsajos "Azure" portale.
  - Atkreipkite dėmesį, kad mūsų paslauga yra tik apie vartotojų/grupių pokyčius šaltinio sistemoje ("Azure Active Directory"). Jei vartotojas/grupė pašalinama tiesiogiai taikomojoje programoje (pvz., ServiceNow), mes nežinome apie tuos keitimus ir nepervyniokite jo pagal šaltinio sistemoje esančio vartotojo būseną. Pagal šį scenarijų geriausia atšaukti pakeitimą tikslinėje taikomojoje programoje.
- Mūsų tarnyba vertino vartotoją/grupę ir nustatė, kad ji neturėtų būti parengta:
  - Jei nustatysite sritį priskirtiems vartotojams ir grupėms, patikrinkite, ar vartotojas/grupė priskiriama taikomajai programai.
  - Jei vartotojas/grupė priskiriama taikomajai programai, įsitikinkite, kad jos nepriskirtos numatytajam prieigos vaidmeniui. Šiam vaidmeniui negalima naudoti parengimo.
  - Jei nustatėte atributą pagal aprėpties filtrą, įsitikinkite, kad vartotojas atitinka nurodytus kriterijus.
  - Jei vartotojai jau yra tikslinėse sistemose ir vartotojo būsena šaltinio ir paskirties atitikmuo, mes nesiimsime jokių tolesnių veiksmų.
- Mūsų tarnyba bandė pateikti vartotojui ir nepavyko. Šiuose scenarijuose Peržiūrėkite parengimo žurnalų skirtuką trikčių diagnostika ir rekomendacijos:
  - Būtinas atributas vartotojui gali trūkti "Azure Active Directory" arba neatitinka trečiosios šalies taikomosios programos reikalaujamos formos. Pvz., šalies atributas vartotojui gali būti nustatytas Jungtinėse Valstijose, kai jis turėtų būti mums.
  - Atributas yra referencinis atributas, kurio dar nėra taikomojoje taikomojoje programoje. Nuorodų atributas yra atributas, kuris nukreipia į kitą objektą, pvz., vartotoją, kuris yra grupės narys. Vartotojo ID būtų grupės nario atributas, tačiau jį galima apdoroti tik tuo atveju, jei vartotojo objektas jau yra.
