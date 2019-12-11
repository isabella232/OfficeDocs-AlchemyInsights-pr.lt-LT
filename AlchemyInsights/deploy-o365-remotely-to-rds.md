---
title: Diegti Office 365 ProPlus bendrai naudoti RDS, terminalo serverio arba VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959467"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Diegti Office 365 ProPlus bendrai naudoti RDS, terminalo serverio arba VDI

Norėdami įdiegti Office 365 ProPlus naudojant nuotolinio darbalaukio tarnybos (RDS), anksčiau pavadintas terminalų tarnybos:
- Turite turėti "Microsoft 365 for Business" planą arba "Office 365" planą, kuriame yra "Office 365 ProPlus", pvz., "Office 365 Enterprise E3" arba "Enterprise E5".
   > [!NOTE] 
   > Office 365 Business "ir" Office 365 "Business Premium" planai neapima "Office 365 ProPlus".
- Turite įgalinti [bendrai kompiuterio aktyvinimas](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Taip pat galite atsisiųsti ir paleisti [Microsoft Support ir atkūrimo asistentas](https://aka.ms/SaRA_OfficeSCA_M365Portal) įdiegti Office 365 ProPlus bendrai naudojamo kompiuterio aktyvinimo režimu.

Daugiau informacijos apie Būtinosios sąlygos, sąrankos instrukcijos ir nurodymai dėl individualų įrenginių naudodami Office visuotinio diegimo įrankį, ieškokite [įdiegti Office 365 ProPlus naudojant nuotolinio darbalaukio tarnybos](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Norėdami ištaisyti klaidas, susijusias su bendrai naudojamo kompiuterio aktyvinimu:
- Peržiūrėkite " [Office 365 ProPlus" bendrai naudojamo kompiuterio aktyvinimo problemų triktis](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Peržiūrėkite [iš naujo nustatyti "Office 365 ProPlus" aktyvinimo būseną](https://go.microsoft.com/fwlink/?linkid=2109218).

Jei norite įdiegti Office 365 ProPlus RDS iš "Microsoft" 365 administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus:

1.  Patikrinkite, ką Office 365 planą turite. [Sužinokite, kaip](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)tai daryti.
2.  Jei reikia, pereikite į kitą Office 365 planą. [Sužinokite, kaip](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)tai daryti.
3.  Jei Office jau yra įdiegta RDS serveryje naudojant kitus Office 365 planus, pašalinkite jį. Pavyzdžiui, eikite į **valdymo skydo** > **išdiegti programą**. Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei jūs naudojate problemų.
4.  RDS serveryje Prisijunkite prie "Microsoft" 365 administravimo centro su savo administratoriaus abonementu ir [įdiekite "Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)".
5.  Įdiegus "Office", ***neatidarykite arba prisijunkite*** prie jokių "Office" taikomųjų programų.
6.  RDS serveryje, įgalinti bendrai kompiuterio aktyvinimas redaguodami registrą atlikdami šiuos veiksmus:
   1. Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite **vykdyti**. Lauke Atidaryti įveskite **regedit**, ir tada pasirinkite **gerai**.
   2. Pasirinkite **taip** Kai paraginama leisti registro rengyklėje atlikti keitimus įrenginyje.
   3. Registro rengyklėje pridėkite eilutės reikšmę **Sharedcomputerlicensing** su parametr 1 pagal HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serveryje, ***Prisijunkite kaip galutiniam vartotojui*** ir [patikrinkite, ar bendrai kompiuterio aktyvinimas yra įjungtas Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

