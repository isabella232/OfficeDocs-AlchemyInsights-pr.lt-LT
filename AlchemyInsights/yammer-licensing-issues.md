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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657284"
---
# <a name="yammer-licensing-issues"></a>"Yammer" licencijavimo problemos

Visi vartotojai turi turėti licenciją, kad galėtų naudoti "Yammer Enterprise" paslaugą, tačiau pagal numatytuosius "Yammer" nereikalauja, kad vartotojai turėtų licenciją, kad galėtų pasiekti paslaugą. Kai administratorius pakeis nustatymą, kad būtų galima blokuoti "Microsoft 365" vartotojus, neturinčius "Yammer" licencijų, vartotojai, kuriems nepriskirta "Yammer Enterprise" licencija, negali pasiekti "Yammer" Daugiau informacijos ieškokite " [Yammer" vartotojų licencijų valdymas "Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) " 

Kai licencijos pašalinamos iš vartotojų, "Yammer" plytelė nebebus rodoma, o kitos tarnybos gali naudoti licencijos pašalinimą, kad būtų slepiamos funkcijos. Kitais atvejais funkcijos vis tiek gali atsirasti, bet reikia vykdyti licencijos priskyrimą.  

**Licencija neatnaujinama vartotojui**  

Kartais vartotojui priskiriama licencija, tačiau jis vis tiek negali pasiekti "Yammer". Delsimas yra labiau tikėtinas, kai vykdoma masinės licencijos priskyrimas. "Yammer" vartotojai gali būti neatnaujinti ta pačia tvarka, kaip licencijos pakeistos "Azure AD", nes sistema veikia asinchroniškai. Palaukite iki 24 valandų, kol bus atidaroma palaikymo byla, kad būtų galima pranešti apie licencijos sinchronizavimo problemas.  

**Masinis licencijų priskyrimas**  

Licencijas galima priskirti administravimo centre arba "PowerShell" scenarijams. Daugiau informacijos ieškokite [licencijų priskyrimas vartotojams](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ir [licencijų priskyrimas vartotojų abonementams su "Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)". 

"Microsoft" palaikymas neteikia pagalbos kuriant scenarijus, bet galima naudoti dokumentaciją apie "Yammer" licencijos priskyrimas. Daugiau informacijos ieškokite ["Yammer" licencijų valdymas naudojant "Windows PowerShell"](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).