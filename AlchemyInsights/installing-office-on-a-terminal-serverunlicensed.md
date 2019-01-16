---
title: Diegti "office" Terminal Server - be leidimų
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301916"
---
# <a name="installing-office-on-a-terminal-server"></a>Diegti "Office" terminalo serverio

Diegiant "Office 365 ProPlus" naudodami nuotolinio darbalaukio tarnybų (RDS) Windows Server, vadintas terminalų tarnybos:
  
- Turite "Office 365" planą, kuris apima "Office 365 ProPlus", pvz., Office 365 Enterprise E3 "arba" Enterprise E5. Office 365 Business "ir" Office 365 Business Premium planus neįeina "Office 365 ProPlus".
    
- Jums reikia įgalinti [bendrinamo kompiuterio suaktyvinimą](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Jei norite įdiegti "Office 365 ProPlus" RDS "Office 365" portale ** *kuri naudoja numatytąjį diegimo parametrus* **, atlikite šiuos veiksmus: 
  
1. Patikrinkite, ką turite "Office 365" planą. [Sužinokite daugiau kaip](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Jei reikia, pereiti prie skirtingų "Office 365" planą. [Sužinokite daugiau kaip](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Jei Office yra įdiegta RDS serverio naudojant kitus "Office 365" planus, pašalinkite ją. Pvz., nuėję į valdymo skydo \> pašalinti programą. Pašalinti, jei kyla problemų naudojant ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SARA-OfficeUninstall-Alchemy) . 
    
4. RDS serveriu, prisijunkite prie "Office 365" portale su administratoriaus paskyrą ir [įdiegti "Office 365 ProPlus"](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Po to, kai Office yra įdiegta, ** *ne atidaryti arba prisijunkite* ** į visas Office programas. 
    
6. RDS serverio, kad aktyvinimo bendrai naudojamame kompiuteryje iš registro redagavimą, atlikite šiuos veiksmus:
    
1. Dešiniuoju pelės mygtuku spustelėkite apatiniame kairiajame kampe ekrano "Windows" mygtuką ir pasirinkite paleisti. Lauke Atidaryti įveskite **regedit**, ir pasirinkite Gerai. 
    
2. Pasirinkite taip, kai būsite paprašyti leisti registro redaktorių keisti įrenginio.
    
3. Registro redaktoriaus, pridėti eilutės reikšmė, **SharedComputerLicensing** 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, kuriame. 
    
7. RDS serverio, ** *kaip galutinio vartotojo Prisijunkite* ** ir [patikrinkite aktyvinimo bendrai naudojamame kompiuteryje įgalintas, "Office 365 ProPlus"](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Daugiau informacijos apie būtinųjų sąlygų, sąrankos nurodymus ir patarimus individualų įrenginių naudodami Office diegimo įrankis, žiūrėkite [Diegti Office 365 ProPlus naudodami nuotolinio darbalaukio tarnybos](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Ištaisyti klaidas, susijusias su bendra kompiuterio aktyvinimu, žiūrėkite [trikčių problemas aktyvinamą bendrai naudojamame kompiuteryje, "Office 365 ProPlus"](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

