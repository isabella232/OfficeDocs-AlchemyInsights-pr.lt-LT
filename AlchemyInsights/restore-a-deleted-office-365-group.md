---
title: Panaikintų "Microsoft 365" grupės atkūrimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645139"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Panaikintų "Microsoft 365" grupės atkūrimas

Panaikintų "Microsoft 365" grupių arba "Microsoft Teams" galite atkurti per 30 dienų nuo panaikinimo.

1. Eikite į ["Microsoft 365"](https://aka.ms/RestoreDeletedGroup) administravimo centrą, kad prisiregistruotų prie panaikintų grupių ir komandų sąrašo.

    **Pastaba:** Prisijunkite naudodami paskyrą, priskirtą nuomotojo administratoriui arba grupių administratoriaus vaidmeniui.

1. Pasirinkite panaikinti "Microsoft 365" grupę / "Teams", kuri bus atkurta, ir **spustelėkite atkurti grupę**.

    Jei grupės atkurti negalima dėl nesuderinamo SMTP adreso, naudokite šią komandą, kad rastumėte konfliktą keliantį objektą ir pašalintumėte SMTP adresą:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Pastaba:** Kai kuriais atvejais gali užtrukti iki 24 valandų, kol grupė ir visi jos duomenys bus atkurti.

    Daugiau informacijos arba sužinokite, kaip atkurti grupes naudojant "PowerShell", žr. [Panaikintų "Microsoft 365" grupės atkūrimas.](https://go.microsoft.com/fwlink/?linkid=867802)