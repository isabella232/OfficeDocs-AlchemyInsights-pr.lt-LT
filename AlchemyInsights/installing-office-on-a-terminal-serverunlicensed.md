---
title: Biuro diegimas terminalų serveryje - Nelicencijuota
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763225"
---
# <a name="installing-office-on-a-terminal-server"></a>"Office" diegimas terminalų serveryje

Microsoft 365 programėlių įmonėms diegti "Windows Server" naudojant nuotolinio darbalaukio tarnybas (RDS), anksčiau vadintą terminalų tarnybomis:
  
- Turite turėti "Microsoft 365" prenumeratą, kurioje yra "Microsoft 365" programos verslui, pvz., "Office 365 Enterprise E3" arba "Enterprise E5". "Microsoft 365" programos verslui ir "Microsoft 365" programos verslui "Premium" planuose neapima "Microsoft 365" programėlių įmonėms.

- Turite įjungti [bendrinamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Jei norite įdiegti "Microsoft 365 Apps" įmonėms RDS iš "Microsoft 365" administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus.

> [!TIP]
> Taip pat galite atsisiųsti ir paleisti ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SaRA_OfficeSCA_M365Portal) įdiegti "Microsoft 365 Apps" įmonėms bendro naudojimo kompiuterio aktyvinimo režimu.
  
1. Patikrinkite, ką turite "Microsoft 365" prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Jei reikia, perjunkite į kitą "Microsoft 365" prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jei "Office" jau įdiegtas RDS serveryje naudojant kitas "Microsoft 365" prenumeratas, pašalinkite ją. Pavyzdžiui, eikite į \> Valdymo skydas Pašalinti programą. Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo pagalbinę priemonę,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei kyla problemų.

4. RDS serveryje prisijunkite prie "Microsoft 365" administravimo centro naudodami administratoriaus abonementą ir [įdiekite "Microsoft 365 Apps for enterprise".](https://portal.office.com/OLS/MySoftware.aspx)

5. Įdiegę "Office", ***neatidarykite ir neprisijunkite prie*** jokių "Office" taikomųjų programų.

6. RDS serveryje, įgalinti bendro naudojimo kompiuterio aktyvinimo redaguodami registrą, atlikite šiuos veiksmus:

1. Dešiniuoju pelės mygtuku spustelėkite mygtuką "Windows", esantį apatiniame kairiajame ekrano kampe, ir pasirinkite Vykdyti. Lauke Atidaryti įveskite **regedit**, tada pasirinkite Gerai.

2. Pasirinkite Taip, kai būsite paraginti leisti registro rengyklę keisti jūsų įrenginį.

3. Registro rengyklėje įtraukite **SharedComputerLicensing** eilutės reikšmę su parametru 1, esantį HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\ClickToRun\Configuration.

7. RDS ***serveryje, prisijunkite kaip galutinis vartotojas*** ir [patikrinkite, ar bendrai naudojamas kompiuterio aktyvinimas yra įjungtas Microsoft 365 Apps verslui](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Daugiau informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir rekomendacijas dėl tinkintų diegimų naudojant "Office" diegimo įrankį rasite ["Microsoft 365" programėlių diegimas įmonei naudojant nuotolinio darbalaukio tarnybas](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Norėdami ištaisyti klaidas, susijusias su kompiuterio aktyvinimu, peržiūrėkite [Trikčių šalinimas naudojant bendrai naudojamą kompiuterio aktyvinimą, skirtą "Microsoft 365" programėlėms, skirtai įmonei](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  