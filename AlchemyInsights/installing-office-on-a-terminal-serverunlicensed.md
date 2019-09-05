---
title: Office diegimas terminalų serveryje-nelicencijuotos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735397"
---
# <a name="installing-office-on-a-terminal-server"></a>Office diegimas terminalų serveryje

Diegti Office 365 ProPlus Windows Server naudojant nuotolinio darbalaukio tarnybos (RDS), anksčiau pavadintas terminalų tarnybos:
  
- Turite turėti Office 365 planą, kuriame yra Office 365 ProPlus, pvz., Office 365 Enterprise E3 arba Enterprise E5. Office 365 Business "ir" Office 365 "Business Premium" planai neapima "Office 365 ProPlus".

- Turite įgalinti [bendrai naudojamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Jei norite įdiegti Office 365 ProPlus RDS iš "Microsoft" 365 administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus:
  
1. Patikrinkite, ką Office 365 planą turite. [Sužinokite, kaip](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Jei reikia, pereikite į kitą Office 365 planą. [Sužinokite, kaip](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jei Office jau yra įdiegta RDS serveryje naudojant kitus Office 365 planus, pašalinkite jį. Pvz., eikite į valdymo skydo \> išdiegti programą. Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei jūs naudojate problemų.

4. RDS serveryje Prisijunkite prie "Microsoft" 365 administravimo centro su savo administratoriaus abonementu ir [įdiekite "Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)".

5. Įdiegus "Office", ***neatidarykite arba prisijunkite*** prie jokių "Office" taikomųjų programų.

6. RDS serveryje, įgalinti bendrai kompiuterio aktyvinimas redaguodami registrą atlikdami šiuos veiksmus:

1. Apatiniame kairiajame ekrano kampe dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką ir pasirinkite vykdyti. Lauke Atidaryti įveskite **regedit**, ir tada pasirinkite Gerai.

2. Pasirinkite taip, kai paraginama leisti registro rengyklėje atlikti keitimus įrenginyje.

3. Registro rengyklėje pridėkite eilutės reikšmę **Sharedcomputerlicensing** su parametr 1 pagal HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS serveryje, ***Prisijunkite kaip galutiniam vartotojui*** ir [patikrinkite, ar bendrai kompiuterio aktyvinimas yra įjungtas Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Daugiau informacijos apie Būtinosios sąlygos, sąrankos instrukcijos ir nurodymai dėl individualų įrenginių naudodami Office visuotinio diegimo įrankį, ieškokite [įdiegti Office 365 ProPlus naudojant nuotolinio darbalaukio tarnybos](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Norėdami ištaisyti klaidas, susijusias su bendrai naudojamo kompiuterio aktyvinimu, žiūrėkite [trikčių diagnostika bendrai naudojamame kompiuterio aktyvinimui Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  