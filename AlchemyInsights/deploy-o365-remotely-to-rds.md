---
title: "\"Microsoft\" 365 taikomųjų programų, skirtų bendrai naudoti RDS, terminalų serveryje arba VDI, diegimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786285"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>"Microsoft" 365 taikomųjų programų, skirtų bendrai naudoti RDS, terminalų serveryje arba VDI, diegimas

Jei norite įdiegti "Microsoft" 365 taikomąsias programas, skirtas įmonėms, naudojančioms nuotolinio darbalaukio tarnybas (RDS), anksčiau pavadintas terminalo tarnybas:
- Turite turėti "Microsoft 365" verslui planą arba "Office 365" planą, kuris aprėpia "Microsoft 365" taikomąsias programas, skirtas įmonėms, pvz., "Office 365 Enterprise E3" arba "Enterprise E5".
   > [!NOTE] 
   > "Microsoft" 365 taikomosios programos verslui ir "Microsoft 365 Business Premium" standartiniai planai neapima "Microsoft 365" taikomųjų programų įmonėms.
- Turite įgalinti [bendrinamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Taip pat galite atsisiųsti ir paleisti ["Microsoft" palaikymo ir atkūrimo pagalbinę priemonę](https://aka.ms/SaRA_OfficeSCA_M365Portal) , kad įdiegtumėte "microsoft" 365 taikomąsias programas, skirtas įmonės bendrinamo kompiuterio aktyvinimo režimu.

Daugiau informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir patarimus apie tinkintus diegimus naudojant "Office" diegimo įrankį rasite ["Microsoft 365" taikomųjų programų diegimas įmonėms naudojant nuotolinio darbalaukio tarnybas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Norėdami ištaisyti klaidas, susijusias su bendrinamo kompiuterio aktyvinimu:
- ["Microsoft 365" programų, skirtų įmonėms, trikčių šalinimas naudojant bendrinamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Žr. [Iš naujo nustatyti „Microsoft 365“ programas, skirtas „Enterprise Activation“](https://go.microsoft.com/fwlink/?linkid=2109218).

Jei norite įdiegti "Microsoft" 365 taikomąsias programas įmonėms RDS iš "Microsoft 365" administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus:

1.    Patikrinkite, kurią prenumeratą turite. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Jei reikia, perjunkite kitą prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jei "Office" jau yra įdiegtas RDS serveryje, naudodami bet kurias kitas "Microsoft" prenumeratas, pašalinkite ją. Pvz., nuėję į **valdymo skydo**  >  **pašalinti programą**. Pašalinkite ["Microsoft" palaikymo ir atkūrimo pagalbinė priemonė,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei naudojate problemas.
4.    RDS serveryje Prisijunkite prie "Microsoft 365" administravimo centro naudodami savo administratoriaus abonementą ir [įdiekite "microsoft 365" taikomąsias programas, skirtas įmonėms](https://portal.office.com/OLS/MySoftware.aspx).
5.    Įdiegę "Office", ***neatidarykite arba prisijunkite*** prie bet kurios "Office" taikomosios programos.
6.    RDS serveryje įjunkite bendrinamą kompiuterio aktyvinimą redaguodami registrą atlikdami šiuos veiksmus:
   1. Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite **vykdyti**. Lauke Atidaryti įveskite **regedit**, tada pasirinkite **gerai**.
   2. Pasirinkite **taip** , kai būsite paraginti leisti registro rengyklę atlikti jūsų įrenginio keitimą.
   3. Registro rengyklėje įtraukite " **Sharedcomputerlicensing** " eilutės reikšmę su 1 parametru HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serveryje ***Prisijunkite kaip galutinis vartotojas*** ir [patikrinkite, ar įgalintas bendrinamas kompiuterio aktyvinimas "Microsoft" "365" programoms, skirtos įmonėms](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

