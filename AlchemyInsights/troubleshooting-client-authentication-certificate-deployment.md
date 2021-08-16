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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020812"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Kliento autentifikavimo sertifikato diegimo trikčių diagnostika

"Intune" NDES/SCEP ir PKCS/PFX kliento sertifikatų profiliai dažnai naudojami kartu su kitais profilių tipais, pvz., "Wi-Fi", VPN ir el. paštu, kad vartotojai galėtų autentifikuoti įmonės išteklius. Kai šie profilių tipai susieti su kliento sertifikato profiliu, jie priklauso nuo sėkmingo to profilio diegimo.

Pradinės infrastruktūros sąrankai ir susietai kliento sertifikato profilio konfigūracijai dažnai reikia trikčių diagnostikos. Nuoseklios NDES jungties sąrankos ir trikčių šalinimo rekomendacijų, kaip atskirti sertifikatų diegimo problemas, žr.: 

- [Konfigūruoti infrastruktūrą, kad būtų galima palaikyti SCEP naudojant "Intune"](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [SCEP sertifikatų profilių trikčių diagnostikos naudojant ""Microsoft Intune"](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Naudokite nurodotus "PowerShell" scenarijus, kad patvirtintumėte konfigūraciją. Daugiau informacijos žr. ["Intune" sertifikato jungties tikrinimo scenarijai](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Kitos dažnos problemos**

**Kai bandau įdiegti "Intune" sertifikato jungtį NDES jungties serveryje, gaunu pranešimą "Slaptažodžio sertifikato užklausoje patvirtinti negalima. Jis gali būti jau naudojamas. Gaukite naują slaptažodį, kurį norite pateikti naudodami šią užklausą."**  

Šis pranešimas reiškia, kad sertifikato jungties diegimą turite vykdyti kaip administratorius.

Kai kuriose aplinkose serveriai, kuriuose veikia "Intune" sertifikatas, turi naudoti tarpinį serverį, kad prisijungtų prie "Intune", todėl sertifikato jungtis turi naudoti tarpinį serverį. Tam tikromis aplinkybėmis NDES jungtis nepaiso sukonfigūruotų tarpinio serverio parametrų ir gali tekti konfigūruoti tarpinio serverio parametrus, kai jie veikia "LocalSystem" saugos kontekste. 
 
Sprendimas yra paleisti "Internet Explorer" kaip SISTEMĄ ir konfigūruoti tarpinį serverį IE. Iš naujo paleidus "Intune" jungties tarnybą, NDES jungtis prisijungia prie "Intune".

**Vartotojų įrenginiai nebegaus SCEP sertifikatų iš NDES.**

Gali būti, kad kliento autentifikavimo sertifikato, išduoto NDES serveriui ir nurodyto NDES jungties diegimo metu, galiojimas baigėsi arba jo nėra. Norėdami išspręsti problemą: 
 
1. Pašalinkite NDES jungtį.  
2. Naudokite šią informaciją norėdami prašyti naujo kliento autentifikavimo arba serverio autentifikavimo sertifikato: 
 
    - Temos pavadinimas: CN =išorinis fqdn  
    - Temos alternatyvusis pavadinimas (abu būtini): DNS=išorinis fqdn, DNS=internal fqdn 
 
3. Iš naujo įdiekite NDES jungtį naudodami naują sertifikatą.