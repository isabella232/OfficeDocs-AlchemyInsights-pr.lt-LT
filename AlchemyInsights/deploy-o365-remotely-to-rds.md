---
title: "\"Microsoft 365\" programėlių, skirtų bendrai naudoti RDS, terminalų serveryje arba VDI, diegimas"
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507594"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>"Microsoft 365" programėlių, skirtų bendrai naudoti RDS, terminalų serveryje arba VDI, diegimas

Norėdami įdiegti "Microsoft 365" programėlių įmonėms naudojant nuotolinio darbalaukio tarnybas (RDS), anksčiau vadinta terminalų tarnybomis:
- Turite turėti "Microsoft 365" verslui planą arba "Office 365" planą, kuriame yra "Microsoft 365" programos, skirtos įmonei, pvz., "Office 365 Enterprise E3" arba "Enterprise E5".
   > [!NOTE] 
   > "Microsoft 365" programos verslui ir "Microsoft 365 Business Premium Standard" planai neapima "Microsoft 365" programėlių įmonėms.
- Turite įgalinti [bendrai naudojamo kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Taip pat galite atsisiųsti ir paleisti ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SaRA_OfficeSCA_M365Portal) įdiegti "Microsoft 365 Apps" įmonėms bendro naudojimo kompiuterio aktyvinimo režimu.

Daugiau informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir rekomendacijas dėl tinkintų diegimų naudojant "Office" diegimo įrankį rasite ["Microsoft 365" programėlių diegimas įmonei naudojant nuotolinio darbalaukio tarnybas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Norėdami ištaisyti klaidas, susijusias su kompiuterio aktyvinimu:
- Peržiūrėkite [Trikčių šalinimas naudojant bendrai naudojamą kompiuterio aktyvinimą, skirtą "Microsoft 365" programėlėms, skirtai įmonei](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Žr. [Iš naujo nustatyti „Microsoft 365“ programas, skirtas „Enterprise Activation“](https://go.microsoft.com/fwlink/?linkid=2109218).

Jei norite įdiegti "Microsoft 365" programėlių įmonėms RDS iš "Microsoft 365" administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus:

1.    Patikrinkite, kokią prenumeratą turite. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Jei reikia, perjunkite į kitą prenumeratą. [Sužinokite, kaip](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jei "Office" jau įdiegtas RDS serveryje naudojant kitas "Microsoft" prenumeratas, pašalinkite ją. Pavyzdžiui, eikite į **Valdymo skydas**  >  **Pašalinti programą**. Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo pagalbinę priemonę,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei kyla problemų.
4.    RDS serveryje prisijunkite prie "Microsoft 365" administravimo centro naudodami administratoriaus abonementą ir [įdiekite "Microsoft 365 Apps for enterprise".](https://portal.office.com/OLS/MySoftware.aspx)
5.    Įdiegę "Office", ***neatidarykite ir neprisijunkite prie*** jokių "Office" taikomųjų programų.
6.    RDS serveryje, įgalinti bendro naudojimo kompiuterio aktyvinimo redaguodami registrą, atlikite šiuos veiksmus:
   1. Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite **Vykdyti**. Lauke Atidaryti įveskite **regedit**, tada pasirinkite **Gerai**.
   2. Pasirinkite **Taip,** kai būsite paraginti leisti registro rengyklę keisti jūsų įrenginį.
   3. Registro rengyklėje įtraukite **SharedComputerLicensing** eilutės reikšmę su parametru 1, esantį HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\ClickToRun\Configuration.
   4. RDS ***serveryje, prisijunkite kaip galutinis vartotojas*** ir [patikrinkite, ar bendrai naudojamas kompiuterio aktyvinimas yra įjungtas Microsoft 365 Apps verslui](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

