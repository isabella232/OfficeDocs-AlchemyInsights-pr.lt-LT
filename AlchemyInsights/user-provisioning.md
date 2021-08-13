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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971347"
---
# <a name="user-provisioning"></a>Vartotojo parengimas

- Naudokite [parengimo pagal poreikį galimybę,](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) kad būtų galima parengti vartotoją ir gauti išsamią diagnostiką apie veiksmus, kurių buvo imtasi.
- Norėdami šalinti problemas, su kuriomis susiduriate su parengimo vartotojais ir grupėmis metu, žr. trikčių [diagnostikos vadovą Nėra vartotojų parengimo](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Jei pastebite, kad vartotojai nėra parengti, žr. Parengimo [žurnalai (peržiūra)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) "Azure Active Directory" (AD). Ieškokite žurnalo įrašų, susijusių su konkrečiu vartotojui.
- Periodiškai iš naujo paleiskite parengimą, kad visi vartotojai, kurie buvo praleisti ankstesniame parengimo cikle.
- Galbūt vartotojas / grupė nebuvo parengti, nes mūsų tarnyba dar neturėjo galimybės įvertinti vartotojo. Peržiūrėkite rekomendacijas, kiek laiko trunka parengimas, ir eigos juostą parengimo konfigūravimo puslapyje. Jei pastovi būsena, nurodyta papildomos išsamios informacijos skyriuje, yra prieš datą, kai vartotojas buvo sukurtas / atnaujintas / panaikintas, tai reiškia, kad dar neįvertinome vartotojo. Pagal šį scenarijų geriausia palaukti, kol baigsis parengimo tarnyba. Jei pasiekta pastovi būsena, rekomenduojame iš naujo paleisti vartotojo sąsają "Azure" portale.
  - Atkreipkite dėmesį, kad mūsų tarnyba žino tik apie vartotojo / grupės pakeitimus šaltinio sistemoje ("Azure Active Directory"). Jei vartotojas / grupė pašalinama tiesiogiai taikomojoje programoje (pvz., "ServiceNow"), mes nežinome apie šiuos pakeitimus ir neatimsime jų atgal pagal vartotojo būseną šaltinio sistemoje. Tokiu atveju geriausia atšaukti pakeitimą tiesiogiai paskirties programoje.
- Mūsų tarnyba įvertino vartotoją / grupę ir nustatė, kad ji neturėtų būti parengimo:
  - Jei nustatėte priskirtų vartotojų ir grupių aprėptį, patikrinkite, ar vartotojui / grupei priskirta programa.
  - Jei vartotojui / grupei priskirta taikomoji programa, įsitikinkite, kad jis nepriskirtas numatytai prieigos vaidmeniui. Šio vaidmens negalima naudoti parengimui.
  - Jei nustatėte atributu pagrįstą filtravimo filtrą, įsitikinkite, kad vartotojas atitinka jūsų nurodytus kriterijus.
  - Jei vartotojai jau yra paskirties sistemoje, o vartotojo būsena šaltinio ir paskirties atitikmenyje, mes nesiimsime jokių tolesnių veiksmų.
- Mūsų tarnyba bandė parengti vartotoją ir nepavyko. Šių scenarijų atveju peržiūrėkite parengimo žurnalų skirtuką Trikčių šalinimas ir rekomendacijos:
  - Gali būti, kad vartotojui trūksta būtinojo atributo "Azure Active Directory" neatitinka formato, kurio reikalauja trečiosios šalies taikomoji programa. Pvz., vartotojo atributas Šalis gali būti nustatytas kaip Jungtinės Amerikos Valstijos, kai jis turėtų būti JAV.
  - Atributas yra nuorodų atributas, kuris dar nėra paskirties programoje. Nuorodų atributas yra atributas, kuris nurodo kitam objektui, pvz., vartotojui, kuris yra grupės narys. Vartotojo ID būtų grupės nario atribute, bet gali būti apdorojamas tik jei vartotojo objektas, kurį nurodo, kad jis jau yra.
