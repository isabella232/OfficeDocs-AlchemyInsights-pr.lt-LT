---
title: DLP gali reikėti pasirinktinio tipo
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932666"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP gali reikėti pasirinktinio tipo

**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą. Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus. Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.

Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus). Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais. Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.

**DLP gali reikėti pasirinktinio informacijos tipo**

Naudodami duomenų praradimo prevencijos (DLP) strategiją, galite identifikuoti ir apsaugoti slaptus organizacijos duomenis. Kai kuriais atvejais gali reikėti sukurti savo **pasirinktinį** slaptos informacijos tipą, kad apsaugotumėte savo organizacijos duomenis.

Pavyzdžiui, jūsų organizacijai gali reikėti identifikuoti ir apsaugoti darbuotojų TAPATYBĖS AR kitus duomenis tam tikru jūsų organizacijai būdingu formatu. Jei taip, daugiau informacijos rasite šiuose straipsniuose.
  
 **Įtaisytojo slaptos informacijos tipo tinkinimas**
  
Jei įtaisytasis slaptos informacijos tipas atitiktų jūsų poreikius vos keliais patobulinimais, galite [tinkinti įtaisytąjį slaptos informacijos tipą](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Pavyzdžiui, galite pridėti arba pašalinti raktinius žodžius arba pridėti arba pašalinti patvirtinamuosius įrodymus, pvz., datą arba adresą.
  
 **Pasirinktinio slaptos informacijos tipo kūrimas**
  
Tačiau jei jums reikia nustatyti ir apsaugoti kito tipo slaptą informaciją, saugos & atitikties centro vartotojo sąsajoje galite [sukurti tinkintą slaptos informacijos tipą.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
  
**Pasirinktinio slaptos informacijos tipo kūrimas saugos & atitikties centro "PowerShell"**

Galiausiai, jei vartotojo sąsaja nepateikia visų reikiamų parinkčių, galite [sukurti pasirinktinį slaptos informacijos tipą saugos & atitikties centro "PowerShell".](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) Pradėdami nuo XML failo, galite naudoti kiekvieną galimą parinktį.
