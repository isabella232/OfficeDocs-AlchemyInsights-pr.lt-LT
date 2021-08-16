---
title: "\"Yammer\" licencijavimo problemos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989740"
---
# <a name="yammer-licensing-issues"></a>"Yammer" licencijavimo problemos

Visi vartotojai turi turėti licenciją naudoti ""Yammer" Enterprise" tarnybą, tačiau pagal numatytuosius "Yammer" nereikalauja, kad vartotojai turėtų licenciją pasiekti tarnybą. Kai administratorius pakeičia parametrą blokuoti Microsoft 365 vartotojams be "Yammer" licencijų, vartotojai, kuriems nepriskirta ""Yammer" Enterprise" licencija, negali pasiekti "Yammer" tarnybos. Daugiau informacijos žr. ["Yammer" licencijų valdymas Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kai licencijos pašalinamos iš vartotojų, "Yammer" plytelė nebebus rodoma, o kitos tarnybos gali naudoti licencijos pašalinimą, kad paslėptumėte funkcijas. Kitais atvejais funkcijos vis tiek gali būti rodomos, tačiau norint veikti reikia licencijos priskyrimo.  

**Vartotojo licencija neatnaujinamas**  

Kartais vartotojui priskiriama licencija, bet jis vis tiek negali pasiekti "Yammer". Delsa labiau tikėtina, kai vyksta masinis licencijos priskyrimas. "Yammer" vartotojai gali būti neatnaujinami ta pačia tvarka, kaip "Azure AD" pakeistos licencijos, nes sistema veikia asinchroniškai. Palaukite iki 24 valandų, kol atidarysite palaikymo atvejį ir praneškite apie licencijos sinchronizavimo problemas.  

**Masinis licencijos priskyrimas**  

Licencijas galima priskirti administravimo centre arba "PowerShell" scenarijuose. Daugiau informacijos žr. [Licencijų priskyrimas vartotojams ir](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Licencijų priskyrimas vartotojų paskyroms naudojant ["Office 365 PowerShell".](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

"Microsoft" palaikymas nesuteikia pagalbos kuriant scenarijus, tačiau galima "Yammer" licencijų priskyrimo dokumentaciją. Daugiau informacijos [žr. Licencijų "Yammer" valdymas naudojant Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).