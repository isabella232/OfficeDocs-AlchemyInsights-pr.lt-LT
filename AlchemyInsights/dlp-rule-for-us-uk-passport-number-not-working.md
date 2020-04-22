---
title: Neveikia JAV / JUNGTINĖS Karalystės paso numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714994"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemos su DLP - JAV / JK pasų numeriai

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

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
  