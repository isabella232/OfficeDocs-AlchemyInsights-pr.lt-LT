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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041014"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>""Microsoft 365" programos įmonėms" diegimas bendrinamam naudojimui RDS, terminalo serveryje arba VDI

Norėdami diegti ""Microsoft 365" programos" naudodami nuotolinio darbalaukio tarnybas (RDS), buvusias terminalo tarnybas, turite:

- Naudokite paprastą pataisą, kad įgalintumėte TLS 1.2 kaip numatytąją reikšmę, jei naudojate senesnę "Windows" versiją (pvz., "Windows 7" SP1, "Windows Server 2008 R2"). Jei reikia paprasto taisymo ir daugiau informacijos, žr. Naujinimas, skirtas [įgalinti TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" Windows](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- Turite planą, kuriame yra "Microsoft 365" programos įmonėms (anksčiau Office 365 Plus"). Pvz., "Office 365 E3" arba "Microsoft 365 E5" arba bet kuris planas, kuriame yra "Project" arba "Visio" kompiuterio versija, pvz., ""Project" 3 planas" arba ""Visio" 2 planas", arba "Microsoft 365 Business Premium" planas, kuriame taip pat yra "Microsoft 365" programos verslui.
- Įgalinti bendrinamo kompiuterio aktyvinimą. Daugiau informacijos žr. [Bendrinamo kompiuterio aktyvinimo naudojant ""Microsoft 365" programos" apžvalga.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Pastaba:** norėdami įdiegti "Microsoft 365" programos kompiuterio aktyvinimo režimu, atsisiųskite ir paleiskite ["Microsoft palaikymo ir atkūrimo pagalbinė priemonė"](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Išsamios informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir rekomendacijas, kaip tinkinti diegimus naudojant "Office" diegimo įrankį, žr. [""Microsoft 365" programos" diegimas naudojant nuotolinio darbalaukio tarnybas.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Norėdami ištaisyti klaidas, susijusias su bendrinamo kompiuterio aktyvinimu, žr.:

- [Bendrinamo kompiuterio aktyvinimo ""Microsoft 365" programos](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Aktyvinimo "Microsoft 365" programos įmonėms nustatymas iš naujo](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Jei norite įdiegti ""Microsoft 365" programos RDS" iš ""Microsoft 365" administravimo centras, kuri naudoja numatytuosius diegimo parametrus, atlikite šiuos veiksmus:

1. Patikrinkite, Microsoft 365 turite planą. Daugiau informacijos [žr. Kokią prenumeratą turiu?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Jei reikia, pereikite į kitą Microsoft 365 planą. Daugiau informacijos žr. [Versijos naujinimas į kitą planą](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Jei "Microsoft 365" programos rds serveryje jau įdiegta naudojant kitus nesuderinamus planus, pašalinkite jį nueidami į **Valdymo**  >  **skydas Pašalinti programą**. Jei kyla problemų, pašalinkite atsisiųsdami ["Microsoft palaikymo ir atkūrimo pagalbinė priemonė.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. RDS serveryje prisijunkite prie ""Microsoft 365" administravimo centras naudodami administratoriaus paskyrą ir įdiekite [Office](https://portal.office.com/OLS/MySoftware.aspx).

   Įdiegę Office, neatidarykite ir neprisijungkite prie Office programų.

1. RDS serveryje įgalinkite bendrinamo kompiuterio aktyvinimą redaguodami registrą:

   1. Dešiniuoju pelės mygtuku spustelėkite Windows mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite **Vykdyti**. Lauke Atidaryti įveskite **regedit**, tada pasirinkite **Gerai**.

   1. Kai būsite paraginti leisti registro rengyklei atlikti keitimus jūsų įrenginyje, pasirinkite **Taip**.

   1. Registro rengyklės dalyje HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration įtraukite **"SharedComputerLicensing"** eilutės reikšmę su **parametru 1.**

1. RDS serveryje prisijunkite kaip galutinis vartotojas ir patikrinkite, ar įjungtas bendrinamo kompiuterio aktyvinimas "Microsoft 365" programos. 

   Daugiau informacijos žr. [Patikrinkite, ar įjungtas bendrinamo kompiuterio aktyvinimas "Microsoft 365" programos.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)