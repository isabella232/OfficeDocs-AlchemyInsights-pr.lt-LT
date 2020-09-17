---
title: Sinchronizuoto vartotojo valdymas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777685"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nepavyksta nustatyti pirminio elektroninio pašto adreso, keisti vartotojo atributus arba pašalinti/naikinti sinchronizuotą vartotoją

Jei katalogų sinchronizavimas įgalintas jūsų aplinkoje, kai kurie vartotojo arba objekto atributai negali būti keičiami naudojant "Microsoft" 365 administravimo centrą.

Norėdami visiškai valdyti sinchronizuotus vartotojus ir visus jų atributus, naudokite vietinius "Active Directory" vartotojus ir grupių valdymo konsolę (Adsiedit. msc).  

Taip pat galite keisti atskirus vartotojus arba atributus sinchronizuotiems vartotojams, naudojantiems "PowerShell", pvz., rodomus šiuose bendruose pavyzdžiuose: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
