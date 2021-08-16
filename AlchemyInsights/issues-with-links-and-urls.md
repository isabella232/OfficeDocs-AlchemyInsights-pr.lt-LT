---
title: Saitų ir URL problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054806"
---
# <a name="issues-with-links-and-urls"></a>Saitų ir URL problemos

Peradresavimo URI / atsakymo URL (abu terminai gali būti naudojami pakaitomis) – tai URL, kuriuos naudoja „Microsoft“ tapatybės platforma, kad pateiktų programos prašomus atpažinimo ženklus. Daugiau informacijos apie šiuos URL žr. toliau pateiktuose straipsniuose:

- [Autentifikavimo srautai ir programų scenarijai](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacija apie peradresavimo URI **programos registracijos** puslapyje kiekvienam scenarijui.
- [Peradresavimo URI / atsakymo URL apribojimai](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nežinau, kaip užregistruoti tinkamą peradresavimo URI / atsakymo URL**

Kai prisijungiate naudodami programą, kurią kuriate, jeigu prisijungimo dialogo langas rodo **AADSTS50011: Prašyme nurodytas url neatitinka url sukonfigūruotų šiai programai <your app ID>**, turėsite įtraukti programos registraciją, peradresavimo URI, kurį naudojo jūsų kodas atpažinimo ženklo prašyme „Microsoft“ tapatybės platformai.

Norėdami įtraukti atsakymo URL, eikite į skirtuką **Autentifikavimas**, esantį jūsų **programos registracijos** puslapyje „Azure“ portale ir įtraukite įrašą dalyje **Peradresavimo URI**. Reikšmė, kurią turite įvesti, priklauso nuo programos, kurią kuriate, tipo, kaip aprašyta žemiau:

- Vieno puslapio programų ir žiniatinklio programų atveju atsakymo URL yra jūsų programos URL. Žr. [vieno puslapio programos registracija](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) arba [žiniatinklio programos registracija naudojant „Azure“ portalą](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Darbalaukio programoms, reikšmė, kurią turite pasirinkti priklauso nuo:
    - platformos („MacOS“ skiriasi nuo „Windows“ arba „Linux“)
    - to, kaip gaunate atpažinimo ženklą (interkatyviai, su įrenginio kodų srautu, su integruotuoju „Windows“ autentifikavimu [IWA] arba su vartotojo vardu / slaptažodžiu).
    Daugiau informacijos žr. [darbalaukio programos – programų registracija – peradresavimo URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobiliųjų įrenginių programose peradresavimo URI priklauso nuo:
    - platformos („iOS“ / „Android“ / „UWP“)
    - informacijos, kuri buvo naudojama kuriant jūsų programą, pvz., „iOS“ grupavimo ID bei „Android“ paketo pavadinimo ir parašo maišos. „Azure“ portalo registracijos programa jums padės. Daugiau informacijos žr. [platformos konfigūravimas ir peradresavimo URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Žiniatinklio API ir kai kurie iš automatinių atpažinimo ženklų gavimo būdų (IWA ir vartotojo vardas / slaptažodis) nereikalauja peradresavimo URI.

**Įdiegiau savo žiniatinklio programą, o kai bandau ją patikrinti, gaunu atsakymo URL neatitikimo pranešimą**

Įtraukite peradresavimo URI visose vietose, kuriose diegiate žiniatinklio programą. Daugiau informacijos žr. [Registruokite žiniatinklio programos programą naudodami „Azure“ portalą](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Įtraukite peradresavimo URI į vietą iškart po to, kai įdiegsite programą toje vietoje.

**Negaliu užregistruoti pakankamai atsakymo URL**

Esate ISV ir turite vieną ar kelis peradresavimo URI kiekvienam savo klientui. Norite perkelti iš ADAL / „Azure AD“ v1.0 į MSAL / „Microsoft“ tapatybės platformą ir pasirodo pranešimas [maksimalus peradresavimo URI skaičius](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Norėdami išspręsti šią problemą, [įtraukite peradresavimo URI į paslaugų principus](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) kurie atitinka kiekvieną iš jūsų klientų.
