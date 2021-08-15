---
title: Automatinis klasifikavimas neveikia taip, kaip tikėtasi, naudojant AIP klientą
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979717"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatinis klasifikavimas neveikia taip, kaip tikėtasi, naudojant AIP klientą

Automatinis klasifikavimas neveikia taip, kaip tikėtasi, naudokite šias rekomenduojamas rekomendacijas:

1. Jei kyla problemų dėl automatinio etikečių žymėjimo, žr. Kaip konfigūruoti automatinio ir rekomenduojamo ["Azure"](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) informacijos apsaugos klasifikacijos sąlygas ir kaip ieškoti [slaptos informacijos tipų.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Patikrinkite, ar naudojate aprėpties strategijas, kurios nėra tinkamai sukonfigūruotos: Kaip konfigūruoti "Azure" informacijos apsaugos strategiją konkretiems vartotojams [naudojant aprėpties strategijas.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Jei automatinis žymėjimas neveikia Outlook, patikrinkite, ar jis nėra apibrėžtas, kaip aprašyta `DRMEncryptProperty` čia: [IRM registro saugos parametrai.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Jei savo ["Azure" informacijos apsaugos strategijai](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) naudojote įtaisytųjų informacijos tipų, patikrinkite, ar jūsų turinys atitinka numatomą formatą.
5. Patikrinkite, ar etiketė tinkamai sukonfigūruota naudojant automatinį **arba** **rekomenduojamą**. (**Automatinis** ženklinimas galimas visose Microsoft 365 programose, **o** rekomenduojamas visoms Microsoft 365, išskyrus Outlook.)
6. Negalite naudoti automatinio klasifikacijos dokumentams ir el. laiškams, kurie anksčiau buvo rankiniu būdu pažymėti arba anksčiau automatiškai pažymėti aukštesne klasifikacija.  Daugiau informacijos žr.: [Kaip taikomos automatinės arba rekomenduojamos etiketės.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Jei vis dar kyla problemų, rinkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus prie palaikymo kvito. Norėdami eksportuoti "Azure" informacijos apsaugos žurnalus:
    - Atidarykite Office dokumentą arba sukurkite naują el. laišką Outlook.
    - Spustelėkite **Apsaugoti / slaptumo**  >  **žinyną ir atsiliepimus.**
    - Spustelėkite **Eksportuoti žurnalus.**
    - Įrašykite žurnalus į savo vietą ir pridėkite juos prie savo tarnybos užklausos.

Papildomos informacijos žr.:

- [Kaip konfigūruoti automatinio ir rekomenduojamo "Azure" informacijos apsaugos klasifikacijos sąlygas](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Bendrųjų scenarijų, kurie naudoja "Azure" informacijos apsaugą, naudojimo instrukcijos](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Peržiūrėkite "Azure" informacijos apsaugos dokumentaciją](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- ["Azure" informacijos apsaugos prenumeratų ir funkcijų peržiūra](https://azure.microsoft.com/pricing/details/information-protection)
- ["Azure" informacijos apsaugos reikalavimai](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- ["Azure" informacijos apsaugos greito pasirengimo pradžia mokymo programa](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Atsisiųsti "Azure" informacijos apsaugos klientą](https://www.microsoft.com/download/details.aspx?id=53018)
