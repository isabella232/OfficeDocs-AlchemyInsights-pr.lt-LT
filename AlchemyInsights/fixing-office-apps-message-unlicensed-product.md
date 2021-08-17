---
title: Aktyvinti „Office“ nepavyko
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893919"
---
# <a name="unable-to-activate-office"></a>Aktyvinti „Office“ nepavyko

**Pastaba:** jei naudojate senesnę "Windows versiją (pvz., "Windows 7"), įsitikinkite, kad TLS 1.2 įgalinta kaip numatytoji. Daugiau informacijos žr. Naujinimas, skirtas [įgalinti TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Patikrinkite, ar jūsų prenumeratos galiojimas nėra pasibaigęs.
- Įsitikinkite, kad turite prenumeratą, leidžiančią naudoti kliento licencijas, pvz., „Office 365 Business“ arba „Business Premium“, ir [įsitikinkite, kad vartotojui yra priskirta licencija](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Įsitikinkite, kad vartotojas prie „Office“ yra prisijungęs su paskyra, kuriai priskirta licencija.
- Peržiūrėkite [„Office 365“ tarnybų sveikatos puslapį](https://docs.microsoft.com/office365/enterprise/view-service-health), kad sužinotumėte, ar yra žinomų tarnybos problemų.
- Patikrinkite užkardos, antivirusinės programos ir tarpinio serverio parametrus, kad užtikrintumėte, jog jie neblokuoja „Microsoft 365“ programų prieigos prie interneto. Žr. [„Office 365“ URL ir IP adresų diapazonai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "„Office 365“ URL ir IP adresų diapazonai").

**Patarimas** „Windows“ kompiuteriuose galime diagnozuoti ir automatiškai už jus išspręsti kelias bendrąsias „Office“ prisijungimo problemas. Atsisiųskite ir paleiskite **[„Microsoft“ palaikymo ir atkūrimo pagalbinę priemonę](https://aka.ms/SaRA-OfficeSignInScenario)**, kad būtų galima naudoti mūsų automatinį įrankį.

Atlikite šiuos problemų sprendimo veiksmus:

- Atidarykite „Office“ taikomąją programą ir [atsijunkite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) nuo bet kokių esamų vartotojų paskyrų. [Pašalinkite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ir [iš naujo priskirkite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) „Office“ licenciją, tada [prisijunkite prie „Office“](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) naudodami paveiktą vartotojo paskyrą.
- Paleiskite [Aktyvinimo trikčių diagnostikos priemonę](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Nustatykite „Office“ aktyvinimo būseną iš naujo](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nustatykite „Office“ aktyvinimo būseną iš naujo")
- [Atlikti „Office“ atkūrimą internete](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Jei reikia papildomų problemų sprendimo patarimų, žr.:  

- [Nelicencijuoto produkto ir aktyvinimo klaidos „Office“](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [„Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau“ klaida, pasirodanti jums aktyvinus „Office“](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)