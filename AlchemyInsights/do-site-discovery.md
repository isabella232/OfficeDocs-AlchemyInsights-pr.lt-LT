---
title: Svetainės aptikimas
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030766"
---
# <a name="do-site-discovery"></a>Svetainės aptikimas

Jei jūsų organizacija vis dar naudoja senstelėjusias žiniatinklio taikomąsias programas ir planus naudoti "Internet Explorer" režimą (kurį daro dauguma klientų), turėtumėte atlikti papildomą svetainės aptikimą.

**Jau esate įdiegę senesnę "Microsoft Edge**

Jei jau sukonfigūravote savo įmonės svetainių sąrašą, kad jis veiktų su senesne Microsoft Edge versija, jūsų svetainės aptikimas beveik baigtas. Vienas dalykas, kurį gali tekti padaryti, yra įtraukti neutralias svetaines.

Neutralios svetainės paprastai yra svetainės, kurios teikia bendrąją ausinę (SSO). Jei iš "Microsoft Edge" nueisite į neutralią svetainę, tada norite likti Microsoft Edge autentifikuoti. Jei pereisite į neutralią svetainę "Internet Explorer" režimu, tada norite likti "Internet Explorer" režimu, kad autentifikuoti.

Identifikuokite visas SSO ar kitas neutralias svetaines, kurias naudojate, ir įtraukite į savo įmonės svetainių sąrašą.

**"Internet Explorer" yra numatytoji naršyklė**

Jei naudojate tik "Internet Explorer", galbūt nežinote, kurios svetainės atnaujino į šiuolaikinius žiniatinklio standartus ir kurioms vis tiek reikia "Internet Explorer". Šias svetaines norėsite rasti ir įtraukti į įmonės svetainių sąrašą, kad "Internet Explorer" režimą būtų galima naudoti tik tose svetainėse.

> [!NOTE]
> [Įmonės svetainės aptikimas](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) apranda svetaines, kuriose gali reikėti "Internet Explorer" režimo. Ji gali rinkti duomenis kompiuteriuose, kuriuose veikia "Windows Internet Explorer 8" iš "Internet Explorer 11", "Windows 10", ""Windows 8".1" arba "Windows 7".

**Duomenų analizė**

Kai surinksite svetainės duomenis, rekomenduojame atlikti šį keturių veiksmų procesą duomenims analizuoti:
1. Rikiuoti duomenis pagal domeną, tada pagal URL.
2. Apibrėžkite taikomosios programos, kuri konfigūruoja "Internet Explorer" režimą, ribas. Norite įtraukti visas svetaines ir žiniatinklio valdiklius, kurie apibrėžia taikomąją programą, bet nenorite įtraukti papildomų svetainių ir valdiklių. Kai kurios svetainės gali būti *https://contoso.com/app1* paprastos, o kitos gali reikalauti apibrėžti kelias svetaines ir puslapius.
3. Patikrinkite taikomąją programą, kad patikrinsite, ar ji neveikia. Daugelis svetainių pasiūlys modernų turinį, kai aptiks modernią naršyklę ir pasiūlys senstelėjusį turinį, kai aptiks "Internet Explorer".
4. Jei nepavyksta patikrinti, įtraukite taikomąją programą į savo įmonės svetainių sąrašą.

> [!NOTE]
> Geriausia sugrupuoti visas svetaines, kurias sudaro programa. Tokiu būdu atnaujinus taikomąją programą, lengviau pašalinti visą svetainę iš "Internet Explorer" režimo ir pradėti naudoti šiuolaikinę tos programos naršyklę.

Kai baigsite svetainės aptikimą ir išanalizuosite duomenis, būsite pasirengę pradėti ieškoti kanalo strategijos.

