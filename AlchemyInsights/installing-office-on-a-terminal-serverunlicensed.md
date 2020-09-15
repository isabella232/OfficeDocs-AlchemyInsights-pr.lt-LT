---
title: "\"Office\" diegimas terminalo serveryje – nelicencijuotas"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663125"
---
# <a name="installing-office-on-a-terminal-server"></a>"Office" diegimas terminalo serveryje

Diegiant "Microsoft" 365 taikomąsias programas įmonėms "Windows Server", naudojant nuotolinio darbalaukio tarnybas (RDS), anksčiau pavadintas terminalų tarnybos:
  
- Turite turėti "Microsoft" 365 prenumeratą, kuri aprėpia "Microsoft 365" taikomąsias programas įmonėms, pvz., "Office 365 Enterprise E3" arba "Enterprise E5". "Microsoft" 365 taikomosios programos verslui ir "Microsoft 365" verslui priemokų planams neapima "Microsoft 365" taikomųjų programų įmonėms.

- Reikia įjungti [bendrinamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jei norite įdiegti "Microsoft" 365 taikomąsias programas įmonėms RDS iš "Microsoft 365" administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite toliau nurodytus veiksmus.

> [!TIP]
> Taip pat galite atsisiųsti ir paleisti ["Microsoft" palaikymo ir atkūrimo pagalbinę priemonę](https://aka.ms/SaRA_OfficeSCA_M365Portal) , kad įdiegtumėte "microsoft" 365 taikomąsias programas, skirtas įmonės bendrinamo kompiuterio aktyvinimo režimu.
  
1. Patikrinkite, kokią "Microsoft" 365 prenumeratą turite. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Jei reikia, perjunkite kitą "Microsoft" 365 prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jei "Office" jau yra įdiegtas RDS serveryje naudodami kitas "Microsoft 365" prenumeratas, pašalinkite ją. Pvz., nuėję į valdymo skydo \> pašalinti programą. Pašalinkite ["Microsoft" palaikymo ir atkūrimo pagalbinė priemonė,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei naudojate problemas.

4. RDS serveryje Prisijunkite prie "Microsoft 365" administravimo centro naudodami savo administratoriaus abonementą ir [įdiekite "microsoft 365" taikomąsias programas, skirtas įmonėms](https://portal.office.com/OLS/MySoftware.aspx).

5. Įdiegę "Office", ***neatidarykite arba prisijunkite*** prie bet kurios "Office" taikomosios programos.

6. RDS serveryje įjunkite bendrinamą kompiuterio aktyvinimą redaguodami registrą atlikdami šiuos veiksmus:

1. Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite vykdyti. Lauke Atidaryti įveskite **regedit**, tada pasirinkite Gerai.

2. Pasirinkite taip, kai būsite paraginti leisti registro rengyklę atlikti jūsų įrenginio keitimą.

3. Registro rengyklėje įtraukite " **Sharedcomputerlicensing** " eilutės reikšmę su 1 parametru HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS serveryje ***Prisijunkite kaip galutinis vartotojas*** ir [patikrinkite, ar įgalintas bendrinamas kompiuterio aktyvinimas "Microsoft" "365" programoms, skirtos įmonėms](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Išsamesnės informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir patarimus apie tinkintus diegimus naudojant "Office" diegimo įrankį, žr. ["Microsoft 365" taikomųjų programų diegimas įmonėms naudojant nuotolinio darbalaukio tarnybas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Norėdami ištaisyti klaidas, susijusias su bendrinamo kompiuterio aktyvinimu, peržiūrėkite triktis, susijusias [su bendrinamo kompiuterio aktyvinimu "Microsoft" 365 programoms Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  