---
title: Kliento autentifikavimo sertifikato diegimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555305"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Kliento autentifikavimo sertifikato diegimo trikčių diagnostika

Intune NDES/SCEP ir PKCS/PFX kliento sertifikatų profiliai paprastai naudojami kartu su kitų tipų profiliais, pvz., "Wifi", "VPN" ir el. paštu, kad vartotojai galėtų autentifikuoti įmonės išteklius. Kai šie profilio tipai yra susiję su kliento sertifikato profilio priklauso nuo sėkmingo diegimo, kad profilis.

Pradiniam infrastruktūros nustatymui ir susijusiai kliento sertifikato profilio konfigūracijai dažnai reikia šalinti triktis. Išsamų vadovą sėkmingai nustatyti NDES jungtis ir trikčių šalinimo patarimų izoliuoti problemas, susijusias su sertifikato diegimas, žr.: 

- [Konfigūruoti infrastruktūrą, palaikančią SCEP su Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Scep sertifikatų profilių trikčių diagnostika naudojant "Microsoft Intune"](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Naudokite nurodytą "PowerShell" scenarijus, kad padėtumėte patikrinti konfigūraciją. Daugiau informacijos ieškokite [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Kitos bendros problemos**

**Kai bandau įdiegti Intune sertifikato jungtį NDES jungties serveryje, gaunu pranešimą" sertifikato užklausos slaptažodžio patikrinti negalima. Jis gali būti naudojamas jau. Gaukite naują slaptažodį, kad pateiktumėte su šia užklausa."**  

Šis pranešimas reiškia, kad turite paleisti sertifikato jungties diegimą kaip administratorius.

Kai kuriose aplinkose, serveriai, kuriuose veikia Intune sertifikatas turi naudoti tarpinį serverį prisijungti prie Intune, ir todėl sertifikato jungtis turi naudoti tarpinį serverį. Tam tikrais atvejais NDES jungtis nepaiso sukonfigūruotų tarpinio serverio parametrų, todėl gali reikėti konfigūruoti tarpinio serverio parametrus vykdant "LocalSystem" saugos kontekstą. 
 
Sprendimas yra paleisti "Internet Explorer" kaip sistemą ir konfigūruoti tarpinį serverį IE. Iš naujo paleidus Intune jungtis paslaugos, NDES jungtis prisijungia prie Intune.

**Vartotojo įrenginiai nebegauja SCEP sertifikatų iš NDES.**

Gali būti, kad kliento autentifikavimo sertifikato, išduoto NDES serverio ir nurodyta NDES jungties diegimo metu, baigėsi arba jo nėra. Norėdami išspręsti: 
 
1. Pašalinti NDES jungtis.  
2. Naudokite šią informaciją norėdami pateikti užklausą dėl naujo kliento autentifikavimo arba serverio autentifikavimo sertifikato: 
 
    - Temos pavadinimas: CN = išorinis fqdn  
    - Tema alternatyvus pavadinimas (abu yra privalomi): DNS = išorinis fqdn, DNS = vidaus fqdn 
 
3. Iš naujo įdiekite NDES jungtis su nauju sertifikatu.