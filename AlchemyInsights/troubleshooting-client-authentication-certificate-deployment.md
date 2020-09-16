---
title: Kliento autentifikavimo sertifikato diegimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658994"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Kliento autentifikavimo sertifikato diegimo trikčių diagnostika

Intune NDES/SCEP ir PKCS/PFX kliento sertifikatų profiliai paprastai naudojami kartu su kitų profilių tipais, pvz., "WiFi", VPN ir el. paštas, kad vartotojai galėtų autentifikuoti įmonės išteklius. Kai šie profilių tipai yra susieti su kliento sertifikato profiliu, priklauso nuo sėkmingo šio profilio diegimo.

Pradinės infrastruktūros sąranka ir susieta kliento sertifikato profilio konfigūracija dažnai reikalauja trikčių diagnostikos. Nuosekliam "NDES" jungties ir trikčių diagnostikos rekomendacijų nustatymui, siekiant izoliuoti problemas, susijusias su sertifikatų įdiegimu, rasite: 

- [Konfigūruokite infrastruktūrą, skirtą "SCEP" su Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- ["SCEP" sertifikatų profilių trikčių šalinimas naudojant "Microsoft Intune"](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Naudokite nurodomus "PowerShell" scenarijus, kad patikrintumėte savo konfigūraciją. Daugiau informacijos ieškokite " [Intune" sertifikato jungties patvirtinimo scenarijuose](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Kitos dažnai pasitaikančių problemų**

**Kai bandau įdiegti Intune sertifikato jungtį "NDES" jungties serveryje, gaunu pranešimą "slaptažodžio sertifikato užklausoje negalima patikrinti. Jis galėjo būti jau panaudotas. Gaukite naują slaptažodį, kad pateiktumėte šią užklausą. "**  

Šis pranešimas reiškia, kad turite vykdyti sertifikato jungties diegimą kaip administratorius.

Kai kuriose aplinkose serveriuose, kuriuose veikia "Intune" sertifikatas, turi būti naudojamas tarpinis serveris, kad prisijungtumėte prie "Intune", todėl sertifikato jungtis turi naudoti tarpinį serverį. Kai kuriais atvejais NDES jungtis nepaiso sukonfigūruotų tarpinio serverio parametrų, todėl gali reikėti sukonfigūruoti tarpinio serverio parametrus "LocalSystem" saugos kontekste. 
 
Sprendimas yra paleisti "Internet Explorer" kaip sistemą ir sukonfigūruoti tarpinį serverį IE. Iš naujo paleidus "Intune Connector" tarnybą, "NDES Connector" prisijungia prie Intune.

**Vartotojų įrenginiai nebegauna SCEP sertifikatų iš NDES.**

Gali būti, kad kliento autentifikavimo sertifikatas, išduotas NDES serveriui ir nurodytas NDES jungties diegimo metu, nebegalioja arba jo nėra. Norėdami išspręsti: 
 
1. Pašalinkite NDES jungtį.  
2. Naudodami šiuos duomenis prašykite naujo kliento autentifikavimo arba serverio autentifikavimo sertifikato: 
 
    - Temos pavadinimas: CN = išorinis FQDN  
    - Tema Alternatyvi Vardas (abu būtini): DNS = išorinis FQDN, DNS = vidinis FQDN 
 
3. Iš naujo įdiekite NDES jungtį su nauju sertifikatu.