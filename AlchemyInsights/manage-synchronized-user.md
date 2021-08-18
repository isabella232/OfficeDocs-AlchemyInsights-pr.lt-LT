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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114786"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nepavyko nustatyti pirminio el. pašto adreso, pakeisti vartotojo atributų arba pašalinti / panaikinti sinchronizuoto vartotojo

Jei katalogų sinchronizavimas įgalintas jūsų aplinkoje, kai kurių vartotojo arba objekto atributų negalima keisti naudojant "Microsoft 365" administravimo centras.

Norėdami visiškai valdyti sinchronizuotus vartotojus ir visus jų atributus, naudokite vietinių active directory vartotojų ir grupių valdymo konsolę (adsiedit.msc).  

Taip pat galite keisti atskirus vartotojus arba sinchronizuotus vartotojus naudodami "PowerShell", pvz., kaip parodyta šiuose bendruosiuose pavyzdžiuose:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
