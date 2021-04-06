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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597451"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Panaikintų "Microsoft 365" grupės atkūrimas

Panaikintų "Microsoft 365" grupių arba "Microsoft Teams" galite atkurti per 30 dienų nuo panaikinimo.

1. Eikite į ["Microsoft 365" administravimo centrą,](https://aka.ms/RestoreDeletedGroup) kad prisiregistruotų, ir išvardikite panaikintas grupes ir komandas.

    **Pastaba:** Prisijunkite naudodami paskyrą, priskirtą nuomotojo administratoriui arba grupių administratoriaus vaidmeniui.

1. Pasirinkite panaikinti "Microsoft 365" grupę / "Teams", kuri bus atkurta, ir **spustelėkite atkurti grupę**.

    Jei grupės atkurti negalima dėl nesuderinamo SMTP adreso, naudokite šią komandą, kad rastumėte konfliktą keliantį objektą ir pašalintumėte SMTP adresą:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Pastaba:** Kai kuriais atvejais gali užtrukti iki 24 valandų, kol grupė ir visi jos duomenys bus atkurti.

    Daugiau informacijos arba sužinokite, kaip atkurti grupes naudojant "PowerShell", žr. [Panaikintų "Microsoft 365" grupės atkūrimas.](https://go.microsoft.com/fwlink/?linkid=867802)