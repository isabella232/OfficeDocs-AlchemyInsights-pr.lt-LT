---
title: Su VPN susijusios problemos
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555233"
---
# <a name="vpn-related-issues"></a>Su VPN susijusios problemos

Sėkmingas VPN ryšio diegimas MDM klientams priklauso nuo įdiegto profilio, kuris teisingai atspindi VPN infrastruktūros reikalavimus. Atitinkamų parametrų kliento platformose, kurį tiriate, žr.: 

["Windows 10" ir "Windows Holographic" įrenginio parametrai VPN ryšiams įtraukti naudojant "Intune"](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[VPN parametrų įtraukimas "iOS" ir "iPadOS" įrenginiuose programoje "Microsoft Intune"](https://docs.microsoft.com/intune/vpn-settings-ios)  
["Android" įrenginio nustatymai konfigūruoti VPN Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[VPN parametrų įtraukimas "macOS" įrenginiuose "Microsoft Intune"](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Jei jūsų VPN profilis naudoja sertifikatu pagrįstą autentifikavimą, įsitikinkite, kad sėkmingai įdiegti šakninis sertifikatas ir kliento autentifikavimo sertifikato profiliai, susieti su VPN profiliu.

**Dažniausiai pasitaikančios problemos**

**Aš įdiegiau VPN profilį įrenginyje. "Intune" rodo, kad jis buvo sėkmingas, tačiau įrenginys neprisijungia prie VPN.**

Sėkminga būsena reiškia, kad "Intune" sėkmingai įdiegė profilį kaip sukonfigūruotas. Tačiau šios konfigūracijos gali neatitikti tinklo ir (arba) autentifikavimo reikalavimų. Peržiūrėkite žurnalus infrastruktūros ir autentifikavimo tarnybos (VPN serverio ir NPS/Radius serverio) daugiau informacijos apie bandė ryšį. Norint rinkti ir peržiūrėti žurnalus, gali reikėti dirbti su tinklo infrastruktūros komanda arba trečiosios šalies VPN tiekėju.

**Kai konfigūruoju pasirinktinį VPN, skirtą "iOS", kiekvienos programos VPN funkcija nepasiekiama.**

"iOS" įrenginių "Intune" programos VPN šiuo metu galimas konkrečiam teikėjų ir partnerių sąrašui, kuris taip pat turi atitikti sertifikato sąlygas prieš konfigūruodami programos VPN. Daugiau informacijos rasite ["iOS" / "iPadOS" įrenginių nustatymas už programėlę Virtualusis privatusis tinklas (VPN) in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Daugiau informacijos apie visus VPN ryšio tipus in Intune rasite [VPN profilių kūrimas, kad prisijungtumėte prie VPN serverių intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**"iOS" pareikalavus VPN neįsijungia, kai pasiekiamas sukonfigūruotas domenas**

Norėdami patikrinti automatinius VPN parametrus, nustatykite šias reikšmes:

Noriu atlikti šiuos veiksmus: **Įvertinkite kiekvieną bandymą prisijungti** 

Pasirinkite, ar norite prisijungti: **jei reikia, prisijunkite**

Kai vartotojai pasiekia šiuos domenus: **paskirties** *domeno vardas*

Jei pirmiau konfigūracija nesėkminga, pridėkite šį elementą:

Kai šis URL nepasiekiamas, priverskite prisijungti VPN: **BADURL**