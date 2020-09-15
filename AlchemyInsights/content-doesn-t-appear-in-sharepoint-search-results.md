---
title: Turinys nerodomas "SharePoint" ieškos rezultatuose
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713138"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Turinys nerodomas "SharePoint" ieškos rezultatuose

Vadovaukitės šiais trikčių diagnostikos veiksmais, kai numatomas turinys nerodomas ieškos rezultatuose:
  
1. Patikrinkite, ar **svetainė** , kurioje yra numatomas turinys, yra nustatyta leisti turiniui Rodyti ieškos rezultatuose. Atlikite veiksmus, aprašytus skyriuje [svetainės turinio rodymas ieškos rezultatuose](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Patikrinkite, ar **sąraše** ar **bibliotekoje** , kurioje yra numatomas turinys, nustatyta leisti turiniui Rodyti ieškos rezultatuose. Atlikite veiksmus, aprašytus skyriuje [turinio rodymas sąrašuose arba bibliotekose ieškos rezultatuose](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Patikrinkite, ar puslapio, dokumento arba pasirinktinio puslapio maketas publikuojamas kaip **pagrindinė versija.** Atlikdami 3 veiksmą [ieška nepateikia visų "SharePoint Online" rezultatų](https://go.microsoft.com/fwlink/?linkid=874525).

4. Patikrinkite, ar vartotojas turi **teisę** peržiūrėti turinį. Atlikite veiksmus, pateiktus " [SharePoint" teisių lygių supratimas](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Jei ieškos schema buvo pakeista įtraukiant naują valdomą ypatybę, redaguojant valdomą ypatybę arba pašalinus valdomą ypatybę, reikia atlikti aptikimą ir perindeksuoti užklausą. Iš **naujo rodykite** turinį atlikdami veiksmus, pateiktus [rankiniu būdu, kad būtų nuskaitant ir iš naujo indeksuojamos svetainės, bibliotekos arba sąrašo](https://docs.microsoft.com/sharepoint/crawl-site-content). Tai gali šiek tiek užtrukti, palaukite 24 valandas prieš patikrindami rezultatus dar kartą.

Daugiau informacijos ieškokite [turinio įgalinimas svetainėje, kad būtų galima ieškoti](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
