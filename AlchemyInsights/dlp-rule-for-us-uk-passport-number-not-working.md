---
title: DLP taisyklė, skirta JAV / JK paso numeriui, neveikia
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004954"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP problemos – JAV / JK pasų numeriai

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su JAV / JK pasų numeriais**

Ar kyla problemų dėl duomenų **praradimo prevencijos (DLP)** neveikia turiniui, kuriame yra **JAV / JK** paso numeris, kai naudojate DLP slaptos informacijos tipą "O365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, ko ieško DLP strategija, kai ji vertinama.
  
Pvz., **JAV / JK** paso numerio strategijos, sukonfigūruotos 75 % patikimumo lygiu, atveju įvertinami toliau nurodyti duomenys ir jie turi būti aptikti, kad taisyklė paleis
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devyni skaitmenys

- **[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devyni skaitmenys iš eilės

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra "Checksum"

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP strategija yra 75 % užtikrinta, kad ji aptiko šio tipo slaptą informaciją, jei šalia 300 simbolių:

  - Funkcija Func_usa_uk_passport randa turinį, kuris atitinka šabloną.

  - Rastas Keyword_passport žodis.

    Pvz., jav / JK  paso numerio strategijai būtų suaktyvinamas šis pavyzdys: JAV paso numeris 123456789

Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų aptiktas JAV / JK paso numeris, ieškokite šiame straipsnyje: Kokios slaptos informacijos tipai ieško [JAV / JK paso numerio](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Naudodami kitą įtaisytą slaptos informacijos tipą, informacijos apie tai, ko reikia kitiems tipams, ieškokite šiame straipsnyje: Kokio tipo [slaptos informacijos tipų ieškoti](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  