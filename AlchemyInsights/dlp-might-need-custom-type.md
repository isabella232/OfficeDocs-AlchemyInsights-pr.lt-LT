---
title: DLP gali reikėti pasirinktinio tipo
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030802"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP gali reikėti pasirinktinio tipo

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP gali reikėti pasirinktinio informacijos tipo**

Naudodami duomenų praradimo prevencijos (DLP) strategiją, galite nustatyti ir apsaugoti slaptus duomenis organizacijoje. Kai kuriais atvejais gali tekti sukurti savo pasirinktinį **slaptos** informacijos tipą, kad apsaugotumėte organizacijos duomenis.

Pvz., jūsų organizacijai gali tekti identifikuoti ir apsaugoti darbuotojų ID ar kitus duomenis tam tikru organizacijos formatu. Jei taip, daugiau informacijos žr. toliau nurodytus straipsnius.
  
 **Įtaisytųjų slaptos informacijos tipo tinkinimas**
  
Jei įtaisytas slaptos informacijos tipas atitiktų jūsų poreikius vos keliais patobulinimais, galite tinkinti įtaisytą [slaptos informacijos tipą](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Pavyzdžiui, galite įtraukti arba pašalinti raktažodžius arba įtraukti arba pašalinti patvirtinamuosius įrodymus, pvz., datą arba adresą.
  
 **Pasirinktinio slaptos informacijos tipo kūrimas**
  
Tačiau jei reikia nustatyti ir apsaugoti kito tipo slaptą informaciją, galite sukurti pasirinktinį slaptos informacijos tipą saugos informacijos centro & vartotojo sąsają. [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)
  
**Pasirinktinio slaptos informacijos tipo kūrimas "PowerShell" saugos & centre**

Galiausiai, jei vartotojo sąsaja pateikia ne visas reikalingas parinktis, galite sukurti pasirinktinį slaptos informacijos tipą ["PowerShell" saugos & centre](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Pradėdami nuo XML failo, galite naudoti visas galimas parinktis.
