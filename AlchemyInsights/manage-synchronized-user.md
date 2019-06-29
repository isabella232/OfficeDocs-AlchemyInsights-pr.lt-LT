---
title: Valdyti sinchronizuoto vartotojo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380513"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Neįmanoma nustatyti pagrindinį el. pašto adresą arba pakeisti vartotojo atributus

Jei katalogų sinchronizavimo yra įjungta jūsų aplinkoje kai vartotojas ar objekto atributų negalima keisti naudojant administravimo centrą.
Visiškai valdyti sinchronizuota vartotojams ir jų atributus, naudokite savo vietos Aktyvaus katalogo vartotojus ir grupes valdymo pultą (adsiedit.msc).  

Taip pat galite keisti atskirų vartotojų arba atributai sinchronizuota vartotojams naudojant "PowerShell", kaip parodyta šių pavyzdžių: 
- Rinkinys-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Rinkinys-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Bandomojo vartotojo" - pavardė "Vartotojas"-pavadinimas "Manager"-skyrius "HR"
- Pašalinti-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com