---
title: "\"Office\" diegimas terminalo serveryje – nelicelicentuotas"
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322007"
---
# <a name="installing-office-on-a-terminal-server"></a>"Office" diegimas terminalo serveryje

Norėdami diegti ""Microsoft 365" programos įmonėms" "Windows" serveryje naudodami nuotolinio darbalaukio tarnybas (RDS), anksčiau vadinus terminalo tarnybas:
  
- Turite turėti "Microsoft 365, kuri apima "Microsoft 365" programos įmonėms, pvz., "Office 365 Enterprise E3" arba "Enterprise E5". Į "Microsoft 365" programos verslui "Microsoft 365" programos verslui Premium planus nėra įtraukta "Microsoft 365" programos įmonėms.

- Turite įgalinti bendrinamo [kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jei norite įdiegti ""Microsoft 365" programos įmonėms RDS" iš ""Microsoft 365" administravimo centras, kuri naudoja ***numatytuosius diegimo parametrus***, atlikite šiuos veiksmus.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Patikrinkite, Microsoft 365 turite prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Jei reikia, pereikite prie kitos Microsoft 365 prenumeratos. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jei Office rds serveryje jau įdiegtas naudojant bet kurią kitą Microsoft 365 prenumeratą, pašalinkite ją. Pvz., nueikite į Valdymo \> skydas Pašalinti programą. Pašalinkite [naudodami "Microsoft palaikymo ir atkūrimo pagalbinė priemonė",](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei kyla problemų.

4. RDS serveryje prisijunkite prie ""Microsoft 365" administravimo centras naudodami administratoriaus paskyrą ir įdiekite ["Microsoft 365" programos įmonėms](https://portal.office.com/OLS/MySoftware.aspx).

5. Įdiegę Office, ***neatidarykite ir neprisijungkite*** prie Office programų.

6. RDS serveryje įgalinkite bendrinamo kompiuterio aktyvinimą redaguodami registrą, atlikite šiuos veiksmus:

1. Dešiniuoju pelės mygtuku spustelėkite Windows mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite Vykdyti. Lauke Atidaryti įveskite **regedit**, tada pasirinkite Gerai.

2. Kai būsite paraginti leisti registro rengyklei atlikti keitimus įrenginyje, pasirinkite Taip.

3. Registro rengyklėje įtraukite eilutės reikšmę **SharedComputerLicensing** su parametru 1 dalyje HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS serveryje prisijunkite kaip galutinis vartotojas ir ***patikrinkite,*** ar įjungtas bendrinamo kompiuterio [aktyvinimas "Microsoft 365" programos įmonėms](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Daugiau informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir rekomendacijas apie tinkintus diegimus naudojant "Office" diegimo įrankį, žr. [""Microsoft 365" programos įmonėms" diegimas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)naudojant nuotolinio darbalaukio tarnybas.
  
Norėdami ištaisyti klaidas, susijusias su bendrinamo kompiuterio aktyvinimu, žr. Bendrinamo kompiuterio [aktyvinimo trikčių "Microsoft 365" programos įmonėms](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  