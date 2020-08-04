---
title: "\"Intune\" \"Wi-Fi\" profiliai"
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555314"
---
# <a name="intune-wi-fi-profiles"></a>"Intune" "Wi-Fi" profiliai

Sėkmingas "Wi-Fi" ryšio diegimas MDM klientams priklauso nuo tinkamai įdiegto profilio, kuris atspindi įmonės "Wi-Fi" infrastruktūros reikalavimus. Norėdami peržiūrėti atitinkamus parametrus kliento platformose, kurį tiriate, žr.: 

["Wi-Fi" parametrų įtraukimas įrenginiams, kuriuose veikia "Android" programoje "Microsoft Intune"](https://docs.microsoft.com/intune/wi-fi-settings-android)

["Wi-Fi" parametrų įtraukimas į "Android Enterprise" skirtus ir visiškai valdomus įrenginius programoje "Microsoft Intune"](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

["Wi-Fi" parametrų įtraukimas į "iOS" ir "iPadOS" įrenginius programoje "Microsoft Intune"](https://docs.microsoft.com/intune/wi-fi-settings-ios)

["Wi-Fi" parametrų įtraukimas į "Windows 10" ir naujesnius įrenginius "Intune"](https://docs.microsoft.com/intune/wi-fi-settings-windows)

["Wi-Fi" parametrų importavimas "Windows" įrenginiams "Intune"](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Dažniausiai pasitaikančios problemos**

**Diegiau "Wi-Fi" profilį, kuris priklauso nuo įdiegto sertifikato, nurodyto "Wi-Fi" profilyje. Tačiau konfigūracijos profiliai rodo klaidos būseną.**

Patikrinkite, ar jūsų įrenginys gavo sertifikatą.

1. Intune eikite į **Visi įrenginiai** ir pasirinkite įrenginį > **Įrenginio konfigūraciją**.

2. Patikrinkite, ar visi numatyti profiliai yra išvardyti ir sėkmingai.

3. Jei turite tarpinių sertifikatų "Android" profilyje, įsitikinkite, kad jie įdiegti "Android" įrenginiuose.

    Norėdami patikrinti sertifikato būseną, eikite į **Įrenginio konfigūracijos**  >  **profiliai**  >  **"Android" tarpinių CA**  >  **ypatybės**  >  **Patikimas sertifikatas**.

Jei vis tiek matote klaidų, peržiūrėkite procedūras ir trikčių šalinimo skyrius. Daugiau informacijos ieškokite [SCEP sertifikatų profilių trikčių diagnostika naudojant "Microsoft Intune".](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

**Įrenginyje diegiau "Wi-Fi" profilį. "Intune" rodo, kad jis buvo sėkmingas, tačiau įrenginys neprisijungia prie "Wi-Fi".**

Sėkminga būsena reiškia, kad "Intune" sėkmingai įdiegė profilį kaip sukonfigūruotas. Tačiau šios konfigūracijos gali neatitikti tinklo ir (arba) autentifikavimo reikalavimų. Jei norite gauti daugiau informacijos apie bandė ryšį, peržiūrėti žurnalus infrastruktūros ir autentifikavimo tarnyba (Wi-Fi prieigos taško valdiklyje ir NPS/Radius serveryje). Jums gali tekti dirbti su tinklo infrastruktūros komanda arba trečiosios šalies "Wi-Fi" tiekėju, kad galėtumėte rinkti ir peržiūrėti žurnalus.