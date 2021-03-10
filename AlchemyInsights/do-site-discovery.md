---
title: Svetainių aptikimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693483"
---
# <a name="do-site-discovery"></a>Svetainių aptikimas

Jei jūsų organizacija vis dar naudoja senstelėjusias žiniatinklio programas ir planus naudoti "Internet Explorer" režimą (kurį dauguma klientų), tada reikia atlikti kai kuriuos papildomus svetainių atradimus.

**Jau įdiegėte senesnę "Microsoft Edge" versiją**

Jei jau sukonfigūravote savo įmonės svetainių sąrašą, kad galėtumėte dirbti su senesnė "Microsoft Edge" versija, jūsų svetainės aptikimas beveik baigtas. Reikia įtraukti neutralias svetaines.

Neutralios svetainės paprastai yra svetainės, kurios teikia bendrąją autentifikacija (SSO). Jei einate į neutralią svetainę iš "Microsoft Edge", "Microsoft Edge" norite pasilikti, kad autentifikuotumėte. Jei einate į neutralią svetainę programoje "Internet Explorer", tada norite sustabdyti "Internet Explorer" režimą, kad autentifikuotumėte.

Identifikuokite bet kokias SSO arba kitas neutralias svetaines ir įtraukite jas į savo įmonės svetainių sąrašą.

**"Internet Explorer" yra jūsų numatytoji naršyklė**

Jei dabar naudojate tik "Internet Explorer", jums gali nežinoti, kurios svetainės buvo atnaujintos į šiuolaikinius žiniatinklio standartus ir kurioms vis dar reikia "Internet Explorer". Norite surasti ir įtraukti šias svetaines į įmonės svetainių sąrašą, kad galėtumėte naudoti "Internet Explorer" režimą tik tose svetainėse.

> [!NOTE]
> [Įmonės svetainės aptikimas](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) aptinka svetaines, kurioms gali reikėti "Internet Explorer" režimo. Galima rinkti duomenis kompiuteriuose, kuriuose veikia "Windows Internet Explorer 8", naudojant "Internet Explorer 11" sistemoje "Windows 10", "Windows 8,1" arba "Windows 7".

**Duomenų analizė**

Surinkę svetainių duomenis rekomenduojame atlikti šiuos keturių etapų procesus, kad galėtumėte analizuoti duomenis:
1. Rūšiuokite duomenis pagal domeną, tada pagal URL.
2. Apibrėžkite taikomosios programos ribas, kad sukonfigūruotumėte "Internet Explorer" režimą. Norite įtraukti visas svetaines ir žiniatinklio valdiklius, kurie apibrėžia programėlę, bet nenorite įtraukti papildomų svetainių ir valdiklių. Kai kurios svetainės gali būti taip paprastos, kaip *https://contoso.com/app1* tuo metu, kai kitos gali reikalauti apibrėžti kelias svetaines ir puslapius.
3. Išbandykite taikomąją programą, kad įsitikintumėte, jog ji neveikia gimtoji. Daugelis svetainių pasiūlys šiuolaikinį turinį, kai aptiks šiuolaikinę naršyklę ir pasiūlys tik senstelėjusį turinį, kai aptiks "Internet Explorer".
4. Įtraukite taikomąją programą į savo įmonės svetainių sąrašą, jei ji nepateikia bandymų.

> [!NOTE]
> Geriausia praktika – grupuoti visas svetaines, kurios susideda iš programos. Tokiu būdu naujinant taikomąją programą lengviau pašalinti visą svetainę iš "Internet Explorer" režimo ir pradėti naudoti šiuolaikinę tos programos naršyklę.

Kai atliksite svetainių atradimą ir išanalizavote duomenis, esate pasirengę pradėti ieškoti kanalo strategijos.

