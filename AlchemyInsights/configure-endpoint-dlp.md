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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402440"
---
# <a name="configure-endpoint-dlp"></a>Konfigūruokite galutinio punkto DLP

„Microsoft“ galinio punkto DLP leidžia išplėsti DLP apsaugą ir stebėjimo galimybes iki slaptos informacijos „Windows 10“ įrenginiuose. Kai įrenginiai parengti įrenginių valdymui, galite sukurti DLP strategijas, kad įgalintumėte elementų apsaugojimo veiksmus. Veiklos naršyklę galima naudoti slaptų elementų veiklai stebėti. Daugiau informacijos žr. [Įrenginių parengimas įrenginių valdymui](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Norėdami pradėti naudoti galinio punkto DLP:

- Įsitikinkite, kad turite atitinkamą SKU / prenumeratų licencijavimą. Daugiau informacijos žr. [SKU / prenumeratų licencijavimas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Patikrinkite teises, reikalingas įrenginio valdymui įgalinti, prieigai prie parengimo puslapio arba įjungti / išjungti įrenginio stebėjimą. Daugiau informacijos žr. [Teisės](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Parenkite įrenginius įrenginių valdymui, laikantis įrenginių parengimo procedūros. Jei trūksta parinkties „Įrenginio parengimas“ (peržiūra), esančios „M365“ atitikties  **parametruose**, įsitikinkite, kad turite tinkamą anksčiau nurodytą licenciją ir teises. Daugiau informacijos žr. [Įrenginių parengimas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Sukurkite DLP strategiją, kad apsaugotumėte slaptus elementus. Daugiau informacijos žr. [Galinio punkto DLP strategijos scenarijai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Daugiau informacijos apie „Microsoft“ galinio punkto DLP, žr. [Sužinokite apie „Microsoft 365“ galinio punkto duomenų praradimo prevenciją (peržiūra)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Svarbūs duomenų rinkimo veiksmai, jei reikia palaikymo:**

1. Atsisiųskite MDATP kliento analizatoriaus peržiūros versiją iš [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Paleiskite įrankį kaip administratorius iš cmd lango:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Kai būsite paraginti „Įveskite sekimų rinkimo minučių skaičių: “, įveskite minučių skaičių, reikalingą scenarijui paleisti
5. Paleisti scenarijų

Surinkite „Zip“ failo išvestį, kuri bus pateikta palaikymo agentui.
