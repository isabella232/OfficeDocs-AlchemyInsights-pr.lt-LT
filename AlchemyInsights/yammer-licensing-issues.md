---
title: "\"Yammer\" licencijavimo problemos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148314"
---
# <a name="yammer-licensing-issues"></a>"Yammer" licencijavimo problemos

Visi vartotojai turi turėti licenciją naudoti "Yammer Enterprise" paslaugą, tačiau pagal numatytuosius nustatymus "Yammer" nereikalauja, kad vartotojai turėtų licenciją naudotis paslauga. Kai administratorius pakeičia parametrą blokuoti "Microsoft 365" vartotojus be "Yammer" licencijų, vartotojai, kuriems nepriskirta "Yammer Enterprise" licencija, negali pasiekti "Yammer" paslaugos. Daugiau informacijos rasite ["Yammer" vartotojų licencijų valdymas "Office 365"](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kai licencijos pašalinamos iš vartotojų, "Yammer" plytelė neberodomas, o kitos tarnybos gali naudoti licencijos šalinimą funkcijoms slėpti. Kitais atvejais funkcijos vis tiek gali pasirodyti, tačiau joms reikia suteikti licenciją.  

**Licencija neatnaujinama vartotojui**  

Kartais vartotojui priskiriama licencija, bet vis tiek nepavyksta pasiekti "Yammer". Delsa yra labiau tikėtina, kai masinis licencijos priskyrimas vyksta. "Yammer" vartotojai gali būti neatnaujinti ta pačia tvarka, kaip licencijos pakeičiamos Azure AD, nes sistema veikia asinchroniškai. Palaukite iki 24 valandų, kol atidarydami palaikymo atvejį praneškite apie licencijos sinchronizavimo problemas.  

**Masinis licencijų priskyrimas**  

Licencijos gali būti priskirtos per administravimo centrą arba "PowerShell" scenarijus. Daugiau informacijos rasite [Licencijų priskyrimas vartotojams](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ir [Licencijų priskyrimas vartotojų abonementams naudojant "Office 365 PowerShell".](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

"Microsoft" palaikymo tarnyba neteikia pagalbos kuriant scenarijus, bet galima naudoti "Yammer" licencijos priskyrimo dokumentaciją. Daugiau informacijos rasite ["Yammer" licencijų valdymas naudojant "Windows PowerShell".](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)