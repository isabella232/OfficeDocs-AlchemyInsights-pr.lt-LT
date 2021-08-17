---
title: Konfigūruokite galutinio punkto DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892807"
---
# <a name="configure-endpoint-dlp"></a>Konfigūruokite galutinio punkto DLP

„Microsoft“ galinio punkto DLP leidžia išplėsti DLP apsaugą ir stebėjimo galimybes iki slaptos informacijos „Windows 10“ įrenginiuose. Kai įrenginiai parengti įrenginių valdymui, galite sukurti DLP strategijas, kad įgalintumėte elementų apsaugojimo veiksmus. Veiklos naršyklę galima naudoti slaptų elementų veiklai stebėti. Daugiau informacijos žr. [Įrenginių parengimas įrenginių valdymui](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Norėdami pradėti naudoti galinio punkto DLP:

- Įsitikinkite, kad turite atitinkamą SKU / prenumeratų licencijavimą. Daugiau informacijos žr. [SKU / prenumeratų licencijavimas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Patikrinkite teises, reikalingas įrenginio valdymui įgalinti, prieigai prie parengimo puslapio arba įjungti / išjungti įrenginio stebėjimą. Daugiau informacijos žr. [Teisės](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Parenkite įrenginius įrenginių valdymui, laikantis įrenginių parengimo procedūros. Daugiau informacijos žr. [Įrenginių parengimas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Sukurkite DLP strategiją, kad apsaugotumėte slaptus elementus. Daugiau informacijos žr. [Galinio punkto DLP strategijos scenarijai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Daugiau informacijos apie „Microsoft“ galinio punkto DLP, žr. [Sužinokite apie „Microsoft 365“ galinio punkto duomenų praradimo prevenciją (peržiūra)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Svarbūs duomenų rinkimo veiksmai, jei reikia palaikymo:**

1. Atsisiųskite [MDATP kliento analizatoriaus peržiūrą.](https://aka.ms/betamdatpanalyzer)
1. Paleiskite įrankį kaip administratorius iš cmd lango:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Kai būsite **paraginti Įvesti minučių skaičių,** kad surinktų sekimą: įveskite minučių, reikalingų scenarijui vykdyti, skaičių.
1. Paleiskite scenarijų.

Surinkite zip failo išvestį, kad ji būtų teikiama palaikymo agentui.
