---
title: Automatinis klasifikavimas neveikia taip, kaip tikėtasi, su AIP klientu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508384"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatinis klasifikavimas neveikia taip, kaip tikėtasi, su AIP klientu

Automatinė klasifikacija neveikia taip, kaip tikėtasi, naudokite šias rekomenduojamas gaires:

1. Jei kyla problemų dėl automatinio ženklinimo, sužinokite, [kaip konfigūruoti automatinio ir rekomenduojamo "Azure" informacijos apsaugos klasifikavimo ir](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ["What the sensitive information types" slaptumo žymų priskyrimo](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)sąlygas .
2. Patikrinkite, ar naudojate aprėpties strategijas, kurios nėra tinkamai sukonfigūruotos: [kaip konfigūruoti konkrečių vartotojų Azure informacijos apsaugos strategiją naudojant aprėpties strategijas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jei automatinis žymėjimas neveikia programoje "Outlook" pridėdami pažymėtą dokumentą, patikrinkite, ar `DRMEncryptProperty` jis nėra apibrėžtas taip, kaip aprašyta čia: [IRM registro parametrai saugai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jei savo "Azure" informacijos apsaugos strategijai naudojote [įtaisytuosius informacijos tipus,](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) patikrinkite, ar jūsų turinys atitinka numatytą formatą.
5. Patikrinkite, ar etiketė tinkamai sukonfigūruota **kaip Automatinis** arba **Rekomenduojama**. (**Automatinis** žymėjimas galimas visoms "Office" programoms, o **rekomenduojama** galima naudoti visose "Office" programose, išskyrus "Outlook".)
6. Negalite naudoti automatinio klasifikavimo dokumentams ir el. laiškams, kurie anksčiau buvo pažymėti rankiniu būdu arba anksčiau automatiškai pažymėti aukštesnia klasifikacija.  Daugiau informacijos rasite: [Kaip taikomos automatinės arba rekomenduojamos etiketės](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jei vis tiek kyla problemų, rinkkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus prie palaikymo bilieto. Norėdami eksportuoti Azure informacijos apsaugos žurnalus:
    - Atidarykite "Office" dokumentą arba sukurkite naują el. laišką programoje "Outlook".
    - Spustelėkite **Apsaugoti / jautrumas**  >  **Žinynas ir atsiliepimai**.
    - Spustelėkite **Eksportuoti žurnalus**.
    - Įrašykite žurnalus į savo vietą ir pridėkite juos prie aptarnavimo užklausos.

Daugiau informacijos rasite:

- [Kaip konfigūruoti sąlygas, automatinio ir rekomenduojamos klasifikacijos Azure informacijos apsaugos](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- ["How-to" vadovai dažniausiai pasitaikančių scenarijų, kurie naudoja Azure informacijos apsauga](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- ["Azure" informacijos apsaugos dokumentų peržiūra](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Peržiūrėkite "Azure" informacijos apsaugos prenumeratas ir funkcijas](https://azure.microsoft.com/pricing/details/information-protection)
- ["Azure" informacijos apsaugos reikalavimai](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- ["Azure" informacijos apsaugos greito pasirengimo darbui pamoka](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Atsisiųskite "Azure" informacijos apsaugos klientą](https://www.microsoft.com/download/details.aspx?id=53018)
