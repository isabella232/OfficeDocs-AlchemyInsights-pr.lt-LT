---
title: Sinchronizuoto vartotojo valdymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823975"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nepavyko nustatyti pirminio el. pašto adreso, pakeisti vartotojo atributų arba pašalinti / panaikinti sinchronizuoto vartotojo

Jei jūsų aplinkoje įgalintas katalogų sinchronizavimas, kai kurių vartotojo arba objekto atributų negalima keisti naudojant "Microsoft 365" administravimo centrą.

Norėdami visiškai valdyti sinchronizuotus vartotojus ir visus jų atributus, naudokite vietinių active directory vartotojų ir grupių valdymo konsolę (adsiedit.msc).  

Taip pat galite keisti atskirus vartotojus arba sinchronizuotus vartotojus naudodami "PowerShell", pvz., kaip parodyta šiuose bendruosiuose pavyzdžiuose:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
