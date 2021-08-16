---
title: "\"\"Microsoft 365\" programos įmonėms\" diegimas bendrinamam naudojimui RDS, terminalo serveryje arba VDI"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031486"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>""Microsoft 365" programos įmonėms" diegimas bendrinamam naudojimui RDS, terminalo serveryje arba VDI

Norėdami diegti ""Microsoft 365" programos įmonėms" naudodami nuotolinio darbalaukio tarnybas (RDS), anksčiau vadinus terminalo tarnybas:

- Turite turėti "Microsoft 365 For Business" planą arba Office 365 planą, kuriame yra "Microsoft 365" programos įmonėms, pvz., "Office 365 Enterprise E3" arba "Enterprise E5".
   > [!NOTE]
   > Į "Microsoft 365" programos verslui Microsoft 365 Business Standard planus nėra įtraukti "Microsoft 365" programos įmonėms.
- Turite įgalinti [bendrinamo kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Taip pat galite atsisiųsti ir paleisti ["Microsoft palaikymo ir atkūrimo pagalbinė priemonė"](https://aka.ms/SaRA_OfficeSCA_M365Portal) norėdami įdiegti "Microsoft 365" programos įmonėms kompiuterio aktyvinimo režimu.

Daugiau informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir rekomendacijas apie tinkintus diegimus naudojant "Office" diegimo įrankį, žr. [""Microsoft 365" programos įmonėms" diegimas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)naudojant nuotolinio darbalaukio tarnybas.

Norėdami ištaisyti klaidas, susijusias su bendrinamo kompiuterio aktyvinimu:

- Žr. [Bendrinamo kompiuterio aktyvinimo trikčių "Microsoft 365" programos įmonėms.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Žr. [Iš naujo nustatyti „Microsoft 365“ programas, skirtas „Enterprise Activation“](https://go.microsoft.com/fwlink/?linkid=2109218).

Jei norite įdiegti ""Microsoft 365" programos įmonėms RDS" iš ""Microsoft 365" administravimo centras, kuri naudoja numatytuosius diegimo ***parametrus,*** atlikite šiuos veiksmus:

1. Patikrinkite, kokią prenumeratą turite. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Jei reikia, pereikite į kitą prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Jei Office rds serveryje jau įdiegtas naudojant kitas "Microsoft" prenumeratas, pašalinkite ją. Pvz., nueikite **į Valdymo**  >  **skydas Pašalinti programą**. Pašalinkite [naudodami "Microsoft palaikymo ir atkūrimo pagalbinė priemonė",](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei kyla problemų.
4. RDS serveryje prisijunkite prie ""Microsoft 365" administravimo centras naudodami administratoriaus paskyrą ir [įdiekite "Microsoft 365" programos įmonėms](https://portal.office.com/OLS/MySoftware.aspx).
5. Įdiegę Office, ***neatidarykite ir neprisijungkite*** prie Office programų.
6. RDS serveryje įgalinkite bendrinamo kompiuterio aktyvinimą redaguodami registrą, atlikite šiuos veiksmus:
   1. Dešiniuoju pelės mygtuku spustelėkite Windows mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite **Vykdyti**. Lauke Atidaryti įveskite **regedit**, tada pasirinkite **Gerai**.
   2. Kai **būsite** paraginti leisti registro rengyklei atlikti keitimus įrenginyje, pasirinkite Taip.
   3. Registro rengyklėje įtraukite eilutės reikšmę **SharedComputerLicensing** su parametru 1 dalyje HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serveryje prisijunkite kaip galutinis vartotojas ir ***patikrinkite,*** ar įjungtas bendrinamo kompiuterio [aktyvinimas "Microsoft 365" programos įmonėms](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
