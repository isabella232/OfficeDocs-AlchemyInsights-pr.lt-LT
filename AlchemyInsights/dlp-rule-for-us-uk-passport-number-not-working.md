---
title: Neveikia JAV / JUNGTINĖS Karalystės paso numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931270"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemos su DLP - JAV / JK pasų numeriai

**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą. Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus. Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.

Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus). Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais. Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.

**DLP problemos su JAV / JK pasų numeriais**

Ar turite problemų su **duomenų praradimo prevencija (DLP)** neveikia turinio, kuriame yra **JAV / JK paso numerį,** kai naudojate DLP slaptos informacijos tipą O365? Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kurios ieškote, kai ji vertinama.
  
Pvz., **JAV ir Jungtinės Karalystės paso numerio** strategija, sukonfigūruota 75 % patikimumo lygiu, įvertinami toliau nurodyti duomenys, kuriuos reikia aptikti, kad taisyklė būtų suaktyvinta
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devyni skaitmenys

- **[Raštas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devyni skaitmenys iš eilės

- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP strategija yra 75% įsitikinusi, kad ji aptiko tokio tipo slaptą informaciją, jei 300 simbolių atstumu:

  - Funkcija Func_usa_uk_passport randa šabloną atitinkantį turinį.

  - Rastas raktinis žodis iš Keyword_passport.

    Pvz., šis pavyzdys būtų sukelti **JAV ir Jungtinės Karalystės paso numerio** politika: JAV paso numeris 123456789

Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų aptiktas JAV/ JUNGTINĖS Karalystės paso numeris, ieškokite šiame šio straipsnio skyriuje: [Kas slaptos informacijos tipai ieško JAV / JUNGTINĖS Karalystės paso numerio](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje
  