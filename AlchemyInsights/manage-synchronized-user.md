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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542005"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Neįmanoma nustatyti pagrindinį el. pašto adresą arba pakeisti vartotojo atributus

Jei katalogų sinchronizavimo yra įjungta jūsų aplinkoje, kai vartotojas ar objekto atributų negalima keisti naudojant "Microsoft" 365 administravimo centro.

Visiškai valdyti sinchronizuota vartotojams ir jų atributus, naudokite savo vietos Aktyvaus katalogo vartotojus ir grupes valdymo pultą (adsiedit.msc).  

Taip pat galite keisti atskirų vartotojų arba atributai sinchronizuota vartotojams naudojant "PowerShell", kaip parodyta šių pavyzdžių: 
- Rinkinys-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Rinkinys-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Bandomojo vartotojo" - pavardė "Vartotojas"-pavadinimas "Manager"-skyrius "HR"
- Pašalinti-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com