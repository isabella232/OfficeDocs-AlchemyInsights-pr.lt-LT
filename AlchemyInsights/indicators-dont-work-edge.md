---
title: Indikatoriai neveikia naudojant "Edge" naršyklę
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326269"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatoriai neveikia naudojant "Edge" naršyklę

Sukūrus indikatorių, jo nepaiso "Edge" ("Smartscreen"). Daugiau informacijos žr. IP ir URL / [domenų indikatorių kūrimas.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1 veiksmas: įsitikinkite, kad:

- Patikrinkite, ar indikatorius teisingas (IP/URL nėra rašybos klaidų, teisingas veiksmas, tinkamos RBAC grupės).
- Sukūrę indikatorių palaukite mažiausiai 2 valandas, kad būtų atsižvelgta į galimą gaišties laiką.
- Įsitikinkite, kad sistema (-os) yra su "Microsoft" sargyba, skirta pabaigos taškui.
- Patikrinkite, ar sistema (-os) gali bendrauti su debesimi.
- Patikrinkite, ar "Smartscreen" įgalintas ir pasiekiamas nueię į [bandomąją svetainę.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2 veiksmas: galimos problemos šalinimas

- Įsitikinkite, kad klientas atitinka reikalavimus. Daugiau informacijos [žr. IP ir URL / domenų indikatorių kūrimas.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Įsitikinkite, kad naudojate naujausią "Edge" naršyklės versiją. Norėdami sužinoti naujausią versiją, [žr. Sužinokite, kurią Microsoft Edge versiją.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Iš naujo paleiskite "Edge" naršyklę.
- Eikite į svetainę, kurios indikatorių turite nustatyti. Jei svetainė nerodoma taip, kaip tikėtasi, pereikite prie 3 veiksmo. 

## <a name="step-3-collect-data"></a>3 veiksmas: duomenų tvarkymas

- Rinkti **MDEClientAnalyzer diagnostikos** duomenis. Instrukcijas [žr. Problemos, susijusios su parengimo mašinomis "Microsoft Defender", skirta "Endpoint".](issues-with-onboarding-machines.md)
- Jei jums patogu įdiegti ir rinkti "Fiddler" sekimą, žr. [Telerik Fiddler](http://www.telerik.com/fiddler).
- Jei norite gauti patarimų iš "Microsoft" palaikymo tarnybą, pasirinkite toliau esančią palaikymo piktogramą, kad atidarytumėte palaikymo atvejį.
