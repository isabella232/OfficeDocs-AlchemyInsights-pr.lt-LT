---
title: "\"DLP\" taisyklė, skirta JAV/JK paso numeris neveikia"
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679232"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemos su DLP-US/UK paso numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**"DLP" problemos su JAV/JK pasų numeriai**

Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **JAV/JK paso numeris** , kai naudojant DLP slaptą informacijos tipą "O365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, kas yra DLP strategija, kai ji vertinama.
  
Pvz., **JAV/JK paso numerio** strategiją, sukonfigūruotą su 75% pasikliovimo lygiu, toliau pateikta informacija vertinama ir turi būti nustatyta taisyklės, kad suaktyvintų
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devyni skaitmenys

- **[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devyni iš eilės skaitmenys

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra jokios kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP strategija yra 75% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:

  - Funkcija Func_usa_uk_passport randa turinį, atitinkantį raštą.

  - Randamas raktažodis iš Keyword_passport.

    Pavyzdžiui, Šis pavyzdys sukeltų **JAV/JK paso numerio** strategiją: JAV paso numeris 123456789

Daugiau informacijos apie tai, ko reikia, kad būtų aptiktas jūsų turinio JAV/JK paso numeris, ieškokite šiame straipsnyje šiame straipsnyje: [kokie jautrūs informacijos tipai tinka JAV/JK paso numeriui](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  