---
title: Su saitais ir URL susijusios problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974469"
---
# <a name="issues-with-links-and-urls"></a>Su saitais ir URL susijusios problemos

Peradresavimo URI/atsakymo URL (abi išraiškos yra pakeičiamos) yra URL, kuriuos naudoja "Microsoft" tapatybės platforma, kad grąžintų programos reikalaujamus atpažinimo ženklus. Informacijos apie šiuos URL ieškokite šiuose straipsniuose:

- [Autentifikavimo srautai ir taikomosios programos scenarijai](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacija apie peradresuojamų URI programos **registracijos** puslapyje kiekvienam scenarijui.
- [Peradresavimo URI/atsakymo URL apribojimai ir apribojimai](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nežinau, kaip užregistruoti tinkamą peradresavimo URI/atsakymo URL savo taikomojoje programoje**

Kai prisijungiate naudodami taikomąją programą, jei prisijungimo dialogo langas rodomas **AADSTS50011: užklausoje nurodytas atsakymo URL nesutampa su taikomąja <your app ID> programa sukonfigūruotais atsakymo URL**, jums reikės įtraukti į savo taikomosios programos registraciją, peradresavimo URI, kurį kodas naudojamas atpažinimo ženklų užklausoje "Microsoft" tapatybės platformoje.

Norėdami įtraukti atsakymo URL, eikite į **autentifikavimo** skirtuką **taikomųjų programų registracijos** puslapyje, esančiame "Azure" portale, ir įtraukite įrašą sekcijoje **peradresuoti Uris** . Peradresuojami URIs (žiniatinklis arba mobilusis/darbalaukis). Reikšmė, kurią reikia įvesti, priklauso nuo pastato, kurį kuriate, tipo, kaip aprašyta toliau:

- Vieno puslapio taikomosiose programose ir žiniatinklio taikomosiose programose atsakymo URL yra jūsų taikomosios programos URL. [Vieno puslapio taikomosios programos registravimas](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) arba žiniatinklio taikomosios programos taikomosios programos registravimas [naudojant "Azure" portalą](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Kompiuterio taikomosiose programose reikšmė, kurią turite pasirinkti, priklauso nuo:
    - platforma (MacOS skiriasi nuo "Windows" arba "Linux")
    - būdas, kaip įgyjate atpažinimo ženklą (interaktyviai, su įrenginio kodo srautu, su integruotu "Windows" autentifikavimu [IWA] arba vartotojo vardu/slaptažodžiu).
    Išsamesnės informacijos ieškokite [kompiuterio programos – programos registracija – peradresavimo URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobiliųjų programų atveju peradresavimo URI priklauso nuo:
    - platforma ("iOS"/"Android"/"UWP")
    - informacija, naudojama jūsų programai kurti, pvz., "iOS" paketo ID, ir paketo pavadinimas ir parašo maiša "Android" "Azure Portal App" registracija padės jums. Išsamesnės informacijos ieškokite [platformos konfigūracija ir peradresavimo URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Žiniatinklio API ir kai kurie tylūs atpažinimo ženklų įsigijimo būdai (IWA ir vartotojo vardas/slaptažodis) nereikalaus peradresavimo URI.

**Įdiegiau žiniatinklio taikomąją programą ir kai išbandžiau įdiegtą taikomąją programą, gaunu atsakymo URL neatitikimo pranešimą**

Įtraukite peradresavimo URI visose vietose, kuriose diegiate žiniatinklio taikomąją programą. Daugiau informacijos rasite [žiniatinklio taikomosios programos taikomosios programos registravimas naudojant "Azure" portalą](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Įtraukti peradresavimo URI vietą iš karto po to, kai įdiegėte taikomąją programą toje vietoje.

**Negaliu užregistruoti pakankamai atsakymo URL**

Esate ISV ir turite vieną ar kelis peradresavimo URI kiekvienam klientui. Norite pereiti iš "ADAL/Azure AD v 1.0" į "MSAL"/"Microsoft" tapatybės platformą ir paspauskite [maksimalų peradresavimo URI skaičių](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Norėdami išspręsti šią problemą, [įtraukite peradresavimo URI į tarnybos principus](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , atitinkančius kiekvieną jūsų klientus.
